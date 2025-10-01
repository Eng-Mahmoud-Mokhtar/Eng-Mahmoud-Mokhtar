import { Github, Mail, Phone, MapPin, GraduationCap, Code, Languages } from "lucide-react";
import { ExperienceCard } from "./components/ExperienceCard";
import { ProjectCard } from "./components/ProjectCard";
import { SkillCategory } from "./components/SkillCategory";
import { Badge } from "./components/ui/badge";
import { Separator } from "./components/ui/separator";
import { Button } from "./components/ui/button";

export default function App() {
  const experiences = [
    {
      company: "TREND SOCIAL",
      role: "Team Lead – Flutter Development",
      period: "Aug 2025 – Present",
      responsibilities: [
        "Led a Flutter team to deliver scalable, high-performance apps",
        "Enhanced apps and optimized UI/UX for better user experience"
      ]
    },
    {
      company: "FREELANCE",
      role: "Flutter Developer | AI Engineer",
      period: "Oct 2023 – Apr 2025",
      responsibilities: [
        "Built custom mobile apps with Flutter tailored to client needs",
        "Integrated AI-driven features to improve functionality"
      ]
    },
    {
      company: "Comma",
      role: "Flutter Developer",
      period: "Oct 2023 – Apr 2025",
      responsibilities: [
        "Developed and optimized mobile apps, improving performance and fixing critical bugs"
      ]
    }
  ];

  const projects = [
    {
      name: "Lumpy Skin Disease",
      description: "App for veterinarians and livestock owners to detect and monitor skin diseases in animals early and accurately.",
      technologies: ["Flutter", "AI/ML", "Image Recognition"]
    },
    {
      name: "BioLock",
      description: "Secures personal items with fingerprint or face verification, ensuring protected access to user data.",
      technologies: ["Flutter", "Biometric Auth", "Security"]
    },
    {
      name: "Cashier",
      description: "Desktop cafe management app handling sales, orders, table status, printing, and order tracking.",
      technologies: ["Flutter", "Desktop", "POS System"]
    },
    {
      name: "WorkZone",
      description: "Biometric attendance app enabling check-ins/check-outs within designated company locations for accurate tracking.",
      technologies: ["Flutter", "Geolocation", "Biometric"]
    },
    {
      name: "Skin Scan Tech",
      description: "Medical app analyzing skin images for accurate diagnosis and personalized treatment, with chatbot support.",
      technologies: ["Flutter", "AI", "Healthcare", "Computer Vision"]
    },
    {
      name: "Kayan",
      description: "Sports app for booking football fields, organizing challenges, connecting with gyms/trainers, and pool reservations.",
      technologies: ["Flutter", "Booking System", "Sports"]
    },
    {
      name: "Building Knowledge",
      description: "Real estate app for buying/selling properties with integrated services and flexible listing subscriptions.",
      technologies: ["Flutter", "Real Estate", "E-commerce"]
    },
    {
      name: "Tamanena",
      description: "Islamic app offering Quran, Duas, Tasbih, Azkar, Friday Sunnah, and location-based prayer times.",
      technologies: ["Flutter", "Islamic", "Geolocation"]
    },
    {
      name: "YIACO",
      description: "Car parking app with valet pickup, parking, return services, secure barcode identification, and real-time updates.",
      technologies: ["Flutter", "Barcode", "Real-time Updates"]
    },
    {
      name: "MoviesApp",
      description: "App for exploring, watching, and downloading movies/series with multiple servers, smart search, and smooth interface.",
      technologies: ["Flutter", "Media Streaming", "Search"]
    },
    {
      name: "OEMDOC",
      description: "Automotive app for Syria, Lebanon, and Jordan for checking cars by chassis, buying/selling parts, and tracking deliveries.",
      technologies: ["Flutter", "Automotive", "E-commerce"]
    },
    {
      name: "Manarah",
      description: "Islamic app providing offline Quran, digital Tasbeeh, Azkar, prayer tracking, Qibla direction, Adhan alerts, and verse reminders.",
      technologies: ["Flutter", "Islamic", "Offline", "Notifications"]
    }
  ];

  const skillCategories = [
    {
      title: "Flutter Development",
      skills: ["UI Implementation", "Clean Architecture", "Performance Optimization"]
    },
    {
      title: "State Management",
      skills: ["Provider", "Bloc", "GetX"]
    },
    {
      title: "Tools & Platforms",
      skills: ["Firebase", "REST APIs", "Postman", "Git", "GitHub"]
    },
    {
      title: "UI/UX Design",
      skills: ["Figma (Intermediate)"]
    },
    {
      title: "Soft Skills",
      skills: ["Problem-solving", "Team Collaboration", "Communication", "Creative Thinking"]
    }
  ];

  return (
    <div className="min-h-screen bg-background">
      {/* Hero Section */}
      <section className="border-b">
        <div className="max-w-6xl mx-auto px-6 py-16">
          <div className="flex items-start justify-between flex-wrap gap-6">
            <div className="space-y-4 flex-1 min-w-[300px]">
              <div className="flex items-center gap-3">
                <div className="w-16 h-16 rounded-full bg-primary flex items-center justify-center">
                  <Code className="w-8 h-8 text-primary-foreground" />
                </div>
                <div>
                  <h1 className="text-4xl">Mahmoud Mokhtar</h1>
                  <p className="text-muted-foreground mt-1">Professional Mobile Developer</p>
                </div>
              </div>
              
              <div className="flex flex-wrap gap-4 text-muted-foreground">
                <a href="tel:01017900067" className="flex items-center gap-2 hover:text-foreground transition-colors">
                  <Phone className="w-4 h-4" />
                  <span>01017900067</span>
                </a>
                <a href="mailto:Mahmoudmokhtar2001@gmail.com" className="flex items-center gap-2 hover:text-foreground transition-colors">
                  <Mail className="w-4 h-4" />
                  <span>Mahmoudmokhtar2001@gmail.com</span>
                </a>
                <div className="flex items-center gap-2">
                  <MapPin className="w-4 h-4" />
                  <span>Al Mansoura, Egypt</span>
                </div>
              </div>

              <div>
                <Button asChild variant="default">
                  <a href="https://github.com/Eng-Mahmoud-Mokhtar" target="_blank" rel="noopener noreferrer" className="flex items-center gap-2">
                    <Github className="w-4 h-4" />
                    View GitHub Profile
                  </a>
                </Button>
              </div>
            </div>

            <div className="space-y-2">
              <Badge variant="secondary" className="px-4 py-2">2+ Years Experience</Badge>
              <Badge variant="secondary" className="px-4 py-2">Flutter Expert</Badge>
              <Badge variant="secondary" className="px-4 py-2">AI Engineer</Badge>
            </div>
          </div>
        </div>
      </section>

      {/* Summary Section */}
      <section className="border-b">
        <div className="max-w-6xl mx-auto px-6 py-12">
          <h2 className="mb-6">Summary</h2>
          <p className="text-muted-foreground max-w-3xl leading-relaxed">
            Professional Mobile Developer with 2+ years of experience. Holds a Bachelor's degree in Artificial Intelligence 
            and specializes in developing scalable, high-performance applications. Experienced in integrating smart features 
            and optimizing app performance for seamless user experiences.
          </p>
        </div>
      </section>

      {/* Experience Section */}
      <section className="border-b">
        <div className="max-w-6xl mx-auto px-6 py-12">
          <h2 className="mb-8">Work Experience</h2>
          <div className="space-y-0">
            {experiences.map((exp, index) => (
              <ExperienceCard
                key={index}
                company={exp.company}
                role={exp.role}
                period={exp.period}
                responsibilities={exp.responsibilities}
              />
            ))}
          </div>
        </div>
      </section>

      {/* Education Section */}
      <section className="border-b">
        <div className="max-w-6xl mx-auto px-6 py-12">
          <h2 className="mb-6">Education</h2>
          <div className="flex items-start gap-4 p-6 border rounded-lg">
            <div className="w-12 h-12 rounded-full bg-primary/10 flex items-center justify-center flex-shrink-0">
              <GraduationCap className="w-6 h-6 text-primary" />
            </div>
            <div className="flex-1">
              <h3>Bachelor's Degree in Artificial Intelligence Science</h3>
              <p className="text-muted-foreground mt-1">Faculty of Artificial Intelligence, Kafr El Sheikh University</p>
              <div className="flex items-center gap-4 mt-2">
                <span className="text-muted-foreground">2020 - Aug 2024</span>
                <Badge variant="secondary">Graduated with Very Good</Badge>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Projects Section */}
      <section className="border-b">
        <div className="max-w-6xl mx-auto px-6 py-12">
          <h2 className="mb-2">Projects</h2>
          <p className="text-muted-foreground mb-8">12 innovative mobile applications across various domains</p>
          <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
            {projects.map((project, index) => (
              <ProjectCard
                key={index}
                name={project.name}
                description={project.description}
                technologies={project.technologies}
              />
            ))}
          </div>
        </div>
      </section>

      {/* Skills Section */}
      <section className="border-b">
        <div className="max-w-6xl mx-auto px-6 py-12">
          <h2 className="mb-8">Skills</h2>
          <div className="space-y-6">
            {skillCategories.map((category, index) => (
              <SkillCategory
                key={index}
                title={category.title}
                skills={category.skills}
              />
            ))}
          </div>
        </div>
      </section>

      {/* Languages Section */}
      <section>
        <div className="max-w-6xl mx-auto px-6 py-12">
          <h2 className="mb-6">Languages</h2>
          <div className="flex gap-6">
            <div className="flex items-center gap-3">
              <Languages className="w-5 h-5 text-muted-foreground" />
              <div>
                <p>Arabic</p>
                <p className="text-muted-foreground">Native</p>
              </div>
            </div>
            <Separator orientation="vertical" className="h-12" />
            <div className="flex items-center gap-3">
              <Languages className="w-5 h-5 text-muted-foreground" />
              <div>
                <p>English</p>
                <p className="text-muted-foreground">Intermediate</p>
              </div>
            </div>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="border-t">
        <div className="max-w-6xl mx-auto px-6 py-8 text-center text-muted-foreground">
          <p>© 2025 Mahmoud Mokhtar. All rights reserved.</p>
        </div>
      </footer>
    </div>
  );
}
