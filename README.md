import { motion } from "framer-motion"; import { Card, CardContent } from "@/components/ui/card"; import { Button } from "@/components/ui/button"; import { Facebook, Instagram, Mail } from "lucide-react";

export default function SakibBio() { return ( <div className="bg-gray-950 text-white font-sans"> {/* Hero Section */} <section className="h-screen flex flex-col justify-center items-center text-center px-6"> <motion.h1 initial={{ opacity: 0, y: -50 }} animate={{ opacity: 1, y: 0 }} transition={{ duration: 1 }} className="text-4xl md:text-6xl font-bold mb-4" > Mohammad Saiful Abedin Sakib </motion.h1> <motion.p initial={{ opacity: 0 }} animate={{ opacity: 1 }} transition={{ delay: 0.5, duration: 1 }} className="text-lg md:text-2xl text-gray-300" > Navy Officer ⚓ | Gamer 🎮 | Dream Chaser ✨ </motion.p> </section>

{/* About Me */}
  <section id="about" className="py-20 px-6 max-w-4xl mx-auto">
    <motion.h2
      initial={{ opacity: 0, y: 30 }}
      whileInView={{ opacity: 1, y: 0 }}
      transition={{ duration: 0.8 }}
      className="text-3xl font-bold mb-6 text-center"
    >
      About Me
    </motion.h2>
    <motion.p
      initial={{ opacity: 0 }}
      whileInView={{ opacity: 1 }}
      transition={{ duration: 1 }}
      className="text-gray-300 text-lg leading-relaxed text-center"
    >
      Hi, I’m <span className="font-semibold">Sakib</span> from Bangladesh 🇧🇩. 
      I proudly serve in the <span className="font-semibold">Bangladesh Navy</span>, where discipline, dedication, 
      and service to the nation shape my life. Outside of duty, I’m deeply passionate about 
      technology, fitness, and gaming.
    </motion.p>
  </section>

  {/* Gaming Journey */}
  <section id="gaming" className="py-20 px-6 bg-gray-900">
    <motion.h2
      initial={{ opacity: 0, y: 30 }}
      whileInView={{ opacity: 1, y: 0 }}
      transition={{ duration: 0.8 }}
      className="text-3xl font-bold mb-6 text-center"
    >
      Gaming Journey
    </motion.h2>
    <motion.p
      initial={{ opacity: 0 }}
      whileInView={{ opacity: 1 }}
      transition={{ duration: 1 }}
      className="text-gray-300 text-lg leading-relaxed text-center mb-8"
    >
      I’m a passionate <span className="font-semibold">Mobile Legends: Bang Bang</span> player. 
      I also run a <span className="font-semibold">pilot boosting service</span>, helping players 
      climb ranks with consistent winning streaks. Gaming isn’t just fun—it’s a way to connect, 
      challenge myself, and inspire others.
    </motion.p>
  </section>

  {/* Contact */}
  <section id="contact" className="py-20 px-6 max-w-3xl mx-auto">
    <motion.h2
      initial={{ opacity: 0, y: 30 }}
      whileInView={{ opacity: 1, y: 0 }}
      transition={{ duration: 0.8 }}
      className="text-3xl font-bold mb-6 text-center"
    >
      Let’s Connect
    </motion.h2>
    <div className="flex justify-center gap-6">
      <Button variant="outline" asChild>
        <a href="https://facebook.com" target="_blank" rel="noreferrer">
          <Facebook className="mr-2 h-5 w-5" /> Facebook
        </a>
      </Button>
      <Button variant="outline" asChild>
        <a href="https://instagram.com" target="_blank" rel="noreferrer">
          <Instagram className="mr-2 h-5 w-5" /> Instagram
        </a>
      </Button>
      <Button variant="outline" asChild>
        <a href="mailto:someone@example.com">
          <Mail className="mr-2 h-5 w-5" /> Email
        </a>
      </Button>
    </div>
  </section>

  {/* Footer */}
  <footer className="py-6 text-center text-gray-500 text-sm">
    © {new Date().getFullYear()} Sakib. All rights reserved.
  </footer>
</div>

); }

