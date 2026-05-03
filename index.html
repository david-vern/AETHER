import React, { useState, useEffect, useRef } from 'react';
import { 
  Recycle, HeartPulse, Zap, Play, ArrowRight, ChevronRight, 
  Menu, X, Box, Layers, Globe, Activity, ShieldCheck, 
  Cpu, Droplet, Microscope, Maximize, Clock, FileVideo, Newspaper
} from 'lucide-react';

// --- STYLES & FONTS ---
const styles = `
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600&family=Playfair+Display:ital,wght@0,400;0,600;0,700;1,400&display=swap');

  :root {
    --bg-light: #EDEAE6;
    --text-primary: #1A1A1A;
    --bg-charcoal: #2F2F2F;
    --text-secondary: #6B6B6B;
    --border-accent: #B8AFA6;
    --highlight-gold: #D4AF37;
  }

  body {
    background-color: var(--bg-light);
    color: var(--text-primary);
    font-family: 'Inter', sans-serif;
    -webkit-font-smoothing: antialiased;
    overflow-x: hidden;
  }

  h1, h2, h3, h4, h5, h6, .font-serif {
    font-family: 'Playfair Display', serif;
  }

  /* Animations */
  .fade-in-up {
    opacity: 0;
    transform: translateY(30px);
    transition: opacity 0.8s cubic-bezier(0.16, 1, 0.3, 1), transform 0.8s cubic-bezier(0.16, 1, 0.3, 1);
  }
  
  .fade-in-up.visible {
    opacity: 1;
    transform: translateY(0);
  }

  /* Abstract 3D Cube Animation */
  .scene {
    width: 200px;
    height: 200px;
    perspective: 600px;
  }
  .cube {
    width: 100%;
    height: 100%;
    position: relative;
    transform-style: preserve-3d;
    animation: slowRotate 20s infinite linear;
  }
  .cube__face {
    position: absolute;
    width: 200px;
    height: 200px;
    border: 1px solid var(--border-accent);
    background: rgba(47, 47, 47, 0.05);
    display: flex;
    align-items: center;
    justify-content: center;
    backdrop-filter: blur(2px);
  }
  .cube__face--front  { transform: rotateY(  0deg) translateZ(100px); }
  .cube__face--right  { transform: rotateY( 90deg) translateZ(100px); }
  .cube__face--back   { transform: rotateY(180deg) translateZ(100px); }
  .cube__face--left   { transform: rotateY(-90deg) translateZ(100px); }
  .cube__face--top    { transform: rotateX( 90deg) translateZ(100px); }
  .cube__face--bottom { transform: rotateX(-90deg) translateZ(100px); }

  @keyframes slowRotate {
    0% { transform: translateZ(-100px) rotateX(0deg) rotateY(0deg); }
    100% { transform: translateZ(-100px) rotateX(360deg) rotateY(360deg); }
  }

  /* Custom Scrollbar */
  ::-webkit-scrollbar { width: 8px; }
  ::-webkit-scrollbar-track { background: var(--bg-light); }
  ::-webkit-scrollbar-thumb { background: var(--border-accent); border-radius: 4px; }
  ::-webkit-scrollbar-thumb:hover { background: var(--bg-charcoal); }
`;

// --- ANIMATION WRAPPER ---
const FadeIn = ({ children, delay = 0, className = "" }) => {
  const domRef = useRef();
  const [isVisible, setVisible] = useState(false);

  useEffect(() => {
    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          setVisible(true);
          observer.unobserve(entry.target);
        }
      });
    }, { threshold: 0.1 });
    
    if (domRef.current) observer.observe(domRef.current);
    return () => observer.disconnect();
  }, []);

  return (
    <div 
      ref={domRef} 
      className={`fade-in-up ${isVisible ? 'visible' : ''} ${className}`}
      style={{ transitionDelay: `${delay}ms` }}
    >
      {children}
    </div>
  );
};

// --- DATA STRUCTURES ---
const TOPICS = [
  {
    id: 'sustainability',
    title: 'Sustainable Circular Economy Models',
    shortDesc: 'Minimizing waste through biodegradable materials and on-demand production.',
    icon: <Recycle size={32} strokeWidth={1.5} />,
    heroSubtitle: 'Redefining Manufacturing',
    introText: 'The transition to a circular economy is being accelerated by 3D printing. By utilizing recycled filaments and producing only what is needed, we drastically reduce industrial waste and carbon footprints.',
    process: ['Material Recovery', 'Filament Extrusion', 'On-Demand Printing', 'End-of-Life Recycling'],
    stats: [
      { value: '75%', label: 'Reduction in Material Waste' },
      { value: 'Zero', label: 'Inventory Requirements' },
      { value: '40%', label: 'Lower Carbon Footprint' }
    ],
    features: [
      { icon: <Globe />, title: 'Localized Production', desc: 'Cutting down transportation emissions by printing locally.' },
      { icon: <Layers />, title: 'Material Innovation', desc: 'Creating strong composites from recycled ocean plastics.' },
      { icon: <Activity />, title: 'Lifecycle Tracking', desc: 'Embedded digital twins to monitor material degradation.' },
      { icon: <Box />, title: 'Minimal Packaging', desc: 'Products printed on-site require virtually zero transit packaging.' }
    ]
  },
  {
    id: 'healthcare',
    title: 'Customized Healthcare Solutions',
    shortDesc: 'Bioprinting and patient-specific prosthetics revolutionizing medical care.',
    icon: <HeartPulse size={32} strokeWidth={1.5} />,
    heroSubtitle: 'Precision Patient Care',
    introText: 'From titanium implants perfectly matched to patient scans to the dawn of bioprinted tissues, 3D printing is enabling hyper-personalized healthcare solutions that improve surgical outcomes and patient recovery.',
    process: ['Patient Scanning', 'Digital Modeling', 'Precision Printing', 'Surgical Implantation'],
    stats: [
      { value: '100%', label: 'Patient-Specific Fit' },
      { value: '-60%', label: 'Surgery Time Reduction' },
      { value: '2M+', label: 'Implants Printed Annually' }
    ],
    features: [
      { icon: <ShieldCheck />, title: 'Biocompatibility', desc: 'Using FDA-approved titanium and medical-grade polymers.' },
      { icon: <Microscope />, title: 'Tissue Engineering', desc: 'Pioneering cellular-level printing for organ repair.' },
      { icon: <Maximize />, title: 'Complex Geometries', desc: 'Porous structures that encourage natural bone ingrowth.' },
      { icon: <Cpu />, title: 'Surgical Guides', desc: 'Exact-fit guides for perfect incision and drill accuracy.' }
    ]
  },
  {
    id: 'prototyping',
    title: 'Accelerated Rapid Prototyping',
    shortDesc: 'Compressing R&D timelines from months to mere hours with advanced polymers.',
    icon: <Zap size={32} strokeWidth={1.5} />,
    heroSubtitle: 'Speed to Market',
    introText: 'Innovation waits for no one. 3D printing allows engineering teams to iterate designs daily, failing fast and succeeding faster, bringing complex aerospace and automotive concepts to reality in record time.',
    process: ['Concept Design', 'Rapid Iteration', 'Functional Testing', 'Final Production'],
    stats: [
      { value: '10x', label: 'Faster Iteration Cycles' },
      { value: '90%', label: 'Cost Savings in R&D' },
      { value: '24/7', label: 'Automated Print Farms' }
    ],
    features: [
      { icon: <Clock />, title: 'Same-Day Testing', desc: 'Design in the morning, physical part in hand by afternoon.' },
      { icon: <Box />, title: 'Tooling Elimination', desc: 'Bypass expensive injection molds during the design phase.' },
      { icon: <Droplet />, title: 'Multi-Material', desc: 'Print rigid frameworks and flexible joints in a single pass.' },
      { icon: <Layers />, title: 'Generative Design', desc: 'AI-driven shapes optimized for weight and structural integrity.' }
    ]
  }
];

const NEWS_ITEMS = [
  { title: "The Dawn of 4D Printing", date: "Oct 12, 2026", desc: "Materials that adapt and change shape over time in response to environmental stimuli." },
  { title: "AeroTech's 3D Printed Engine", date: "Sep 28, 2026", desc: "How a single continuous print is revolutionizing deep-space propulsion systems." },
  { title: "Bioprinting Milestone Reached", date: "Sep 15, 2026", desc: "Researchers successfully implant the first fully 3D printed synthetic vascular network." }
];

const VIDEO_ITEMS = [
  { title: "What is 3D Printing?", youtubeId: "a42znmU6BLE" },
  { title: "A Decade of Aerospace Innovation", youtubeId: "q0picmNrFoU" },
  { title: "Next Generation of 3D Printed Surgical Instruments", youtubeId: "2XlHMR01NYA" }
];

// --- COMPONENTS ---

const Navbar = ({ currentView, setView }) => {
  const [isOpen, setIsOpen] = useState(false);

  const navLinks = [
    { id: 'home', label: 'Home' },
    { id: 'media', label: 'Media & News' }
  ];

  return (
    <nav className="sticky top-0 z-50 bg-[#EDEAE6]/90 backdrop-blur-md border-b border-[#B8AFA6]/30">
      <div className="max-w-[1200px] mx-auto px-6 h-20 flex items-center justify-between">
        <div 
          className="flex items-center gap-3 cursor-pointer group"
          onClick={() => setView('home')}
        >
          <div className="w-8 h-8 bg-[#1A1A1A] text-[#D4AF37] flex items-center justify-center rounded-[8px] group-hover:bg-[#2F2F2F] transition-colors">
            <Box size={18} />
          </div>
          <span className="font-serif font-bold text-xl tracking-wide text-[#1A1A1A]">AETHER</span>
        </div>

        {/* Desktop Nav */}
        <div className="hidden md:flex items-center gap-8">
          {navLinks.map(link => (
            <button
              key={link.id}
              onClick={() => setView(link.id)}
              className={`text-sm tracking-widest uppercase transition-colors ${
                currentView === link.id ? 'text-[#1A1A1A] font-semibold' : 'text-[#6B6B6B] hover:text-[#1A1A1A]'
              }`}
            >
              {link.label}
            </button>
          ))}
          <div className="group relative">
            <button className="text-sm tracking-widest uppercase text-[#6B6B6B] hover:text-[#1A1A1A] transition-colors flex items-center gap-1">
              Topics <ChevronRight size={14} className="group-hover:rotate-90 transition-transform" />
            </button>
            <div className="absolute top-full right-0 mt-4 w-64 bg-[#1A1A1A] p-2 rounded-[12px] opacity-0 invisible group-hover:opacity-100 group-hover:visible transition-all shadow-xl">
              {TOPICS.map(topic => (
                <button
                  key={topic.id}
                  onClick={() => setView(topic.id)}
                  className="w-full text-left px-4 py-3 text-[#EDEAE6] text-sm hover:bg-[#2F2F2F] hover:text-[#D4AF37] rounded-[8px] transition-colors"
                >
                  {topic.title}
                </button>
              ))}
            </div>
          </div>
          <button 
            onClick={() => setView('sustainability')}
            className="px-6 py-2.5 bg-[#1A1A1A] text-[#EDEAE6] text-sm tracking-wider uppercase rounded-[10px] hover:bg-[#D4AF37] hover:text-[#1A1A1A] transition-all duration-300"
          >
            Explore
          </button>
        </div>

        {/* Mobile Menu Toggle */}
        <button className="md:hidden text-[#1A1A1A]" onClick={() => setIsOpen(!isOpen)}>
          {isOpen ? <X size={24} /> : <Menu size={24} />}
        </button>
      </div>

      {/* Mobile Nav */}
      {isOpen && (
        <div className="md:hidden absolute top-20 left-0 w-full bg-[#EDEAE6] border-b border-[#B8AFA6] p-6 flex flex-col gap-4">
          <button onClick={() => { setView('home'); setIsOpen(false); }} className="text-left font-serif text-lg border-b border-[#B8AFA6]/30 pb-2">Home</button>
          <button onClick={() => { setView('media'); setIsOpen(false); }} className="text-left font-serif text-lg border-b border-[#B8AFA6]/30 pb-2">Media & News</button>
          <div className="flex flex-col gap-2 pt-2">
            <span className="text-xs tracking-widest text-[#6B6B6B] uppercase mb-2">Topics</span>
            {TOPICS.map(topic => (
              <button 
                key={topic.id}
                onClick={() => { setView(topic.id); setIsOpen(false); }} 
                className="text-left text-[#1A1A1A] text-sm py-1"
              >
                — {topic.title}
              </button>
            ))}
          </div>
        </div>
      )}
    </nav>
  );
};

const Footer = () => (
  <footer className="bg-[#1A1A1A] text-[#EDEAE6] py-16">
    <div className="max-w-[1200px] mx-auto px-6 grid grid-cols-1 md:grid-cols-4 gap-12">
      <div className="md:col-span-2">
        <div className="flex items-center gap-3 mb-6">
          <div className="w-8 h-8 bg-[#2F2F2F] text-[#D4AF37] flex items-center justify-center rounded-[8px]">
            <Box size={18} />
          </div>
          <span className="font-serif font-bold text-xl tracking-wide">AETHER</span>
        </div>
        <p className="text-[#B8AFA6] text-sm max-w-sm leading-relaxed">
          Shaping the future of manufacturing, healthcare, and sustainability through advanced 3D printing technologies and materials.
        </p>
      </div>
      <div>
        <h4 className="font-serif text-[#D4AF37] mb-6">Explore</h4>
        <ul className="space-y-3 text-sm text-[#B8AFA6]">
          <li className="hover:text-[#EDEAE6] cursor-pointer transition-colors">Sustainability</li>
          <li className="hover:text-[#EDEAE6] cursor-pointer transition-colors">Healthcare</li>
          <li className="hover:text-[#EDEAE6] cursor-pointer transition-colors">Prototyping</li>
        </ul>
      </div>
      <div>
        <h4 className="font-serif text-[#D4AF37] mb-6">Connect</h4>
        <ul className="space-y-3 text-sm text-[#B8AFA6]">
          <li className="hover:text-[#EDEAE6] cursor-pointer transition-colors">Media & News</li>
          <li className="hover:text-[#EDEAE6] cursor-pointer transition-colors">Press Kit</li>
          <li className="hover:text-[#EDEAE6] cursor-pointer transition-colors">Contact Us</li>
        </ul>
      </div>
    </div>
    <div className="max-w-[1200px] mx-auto px-6 mt-16 pt-8 border-t border-[#2F2F2F] text-xs text-[#6B6B6B] flex flex-col md:flex-row justify-between items-center">
      <div className="flex flex-col md:flex-row items-center gap-2 text-center md:text-left">
        <p>© 2026 Aether Innovation Labs. All rights reserved.</p>
        <span className="hidden md:inline">•</span>
        <p>Website designed by <span className="text-[#B8AFA6]">Himash Fernando</span></p>
      </div>
      <div className="flex gap-4 mt-4 md:mt-0">
        <span className="hover:text-[#B8AFA6] cursor-pointer">Privacy</span>
        <span className="hover:text-[#B8AFA6] cursor-pointer">Terms</span>
      </div>
    </div>
  </footer>
);

// --- PAGE VIEWS ---

const HomePage = ({ setView }) => (
  <main>
    {/* Hero Section */}
    <section className="py-[100px] px-6 max-w-[1200px] mx-auto grid grid-cols-1 lg:grid-cols-2 gap-16 items-center min-h-[80vh]">
      <FadeIn delay={0}>
        <div className="flex items-center gap-3 mb-6">
          <span className="h-[1px] w-8 bg-[#D4AF37]"></span>
          <span className="text-[#D4AF37] text-xs font-semibold tracking-[0.2em] uppercase">3D Printing Innovation</span>
        </div>
        <h1 className="font-serif text-5xl md:text-7xl font-bold text-[#1A1A1A] leading-[1.1] mb-8">
          The Future of <br />
          <span className="text-[#6B6B6B]">3D Printing</span>
        </h1>
        <p className="text-[#6B6B6B] text-lg max-w-md leading-relaxed mb-10">
          Discover how 3D printing is reshaping industries through sustainability, precision healthcare, and rapid innovation.
        </p>
        <button 
          onClick={() => setView('sustainability')}
          className="group flex items-center gap-4 bg-[#1A1A1A] text-[#EDEAE6] px-8 py-4 rounded-[12px] hover:bg-[#2F2F2F] hover:shadow-[0_10px_30px_rgba(26,26,26,0.15)] transition-all duration-300"
        >
          <span className="tracking-wide uppercase text-sm">Explore Topics</span>
          <ArrowRight size={18} className="text-[#D4AF37] group-hover:translate-x-1 transition-transform" />
        </button>
      </FadeIn>
      
      <FadeIn delay={200} className="hidden lg:flex justify-center items-center h-[400px]">
        {/* CSS Abstract 3D Object */}
        <div className="scene">
          <div className="cube">
            <div className="cube__face cube__face--front"><Box size={48} className="text-[#B8AFA6] opacity-30" /></div>
            <div className="cube__face cube__face--back"><Layers size={48} className="text-[#B8AFA6] opacity-30" /></div>
            <div className="cube__face cube__face--right"></div>
            <div className="cube__face cube__face--left"></div>
            <div className="cube__face cube__face--top"></div>
            <div className="cube__face cube__face--bottom"></div>
          </div>
        </div>
      </FadeIn>
    </section>

    {/* Topics Section */}
    <section className="bg-[#2F2F2F] py-[100px] px-6">
      <div className="max-w-[1200px] mx-auto">
        <FadeIn delay={0}>
          <h2 className="font-serif text-3xl md:text-5xl text-[#EDEAE6] mb-16 text-center">Explore Key Applications</h2>
        </FadeIn>
        
        <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
          {TOPICS.map((topic, index) => (
            <FadeIn delay={index * 150} key={topic.id}>
              <div 
                onClick={() => setView(topic.id)}
                className="bg-[#1A1A1A] p-8 rounded-[12px] border border-[#2F2F2F] cursor-pointer group hover:-translate-y-2 hover:border-[#D4AF37]/50 hover:shadow-[0_10px_30px_rgba(212,175,55,0.05)] transition-all duration-500 h-full flex flex-col"
              >
                <div className="w-14 h-14 bg-[#2F2F2F] rounded-[10px] flex items-center justify-center text-[#D4AF37] mb-6 group-hover:scale-110 transition-transform duration-500">
                  {topic.icon}
                </div>
                <h3 className="font-serif text-xl text-[#EDEAE6] mb-4 leading-snug group-hover:text-[#D4AF37] transition-colors">{topic.title}</h3>
                <p className="text-[#B8AFA6] text-sm leading-relaxed mb-8 flex-grow">{topic.shortDesc}</p>
                <div className="flex items-center text-xs tracking-widest uppercase text-[#6B6B6B] group-hover:text-[#EDEAE6] transition-colors mt-auto">
                  View Detail <ArrowRight size={14} className="ml-2 opacity-0 group-hover:opacity-100 -translate-x-2 group-hover:translate-x-0 transition-all" />
                </div>
              </div>
            </FadeIn>
          ))}
        </div>
      </div>
    </section>

    {/* Featured Section */}
    <section className="py-[100px] px-6 max-w-[1200px] mx-auto">
      <div className="grid grid-cols-1 lg:grid-cols-5 gap-12">
        <FadeIn delay={0} className="lg:col-span-3">
          <div className="flex items-center gap-3 mb-6">
            <span className="h-[1px] w-8 bg-[#1A1A1A]"></span>
            <span className="text-[#1A1A1A] text-xs font-semibold tracking-[0.2em] uppercase">Featured Media</span>
          </div>
          <h2 className="font-serif text-3xl md:text-4xl text-[#1A1A1A] mb-8">What is 3D Printing?</h2>
          
          {/* Embedded YouTube Player */}
          <div className="relative w-full aspect-video bg-[#1A1A1A] rounded-[12px] overflow-hidden border border-[#B8AFA6]">
            <iframe 
              width="100%" 
              height="100%" 
              src="https://www.youtube.com/embed/a42znmU6BLE?rel=0" 
              title="What is 3D Printing?" 
              frameBorder="0" 
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
              allowFullScreen
              className="absolute inset-0"
            ></iframe>
          </div>
        </FadeIn>

        <FadeIn delay={200} className="lg:col-span-2 flex flex-col justify-center">
          <div className="flex items-center justify-between mb-8">
            <h3 className="font-serif text-2xl text-[#1A1A1A]">Latest Insights</h3>
            <button 
              onClick={() => setView('media')}
              className="text-[#6B6B6B] hover:text-[#D4AF37] transition-colors text-sm font-medium"
            >
              View All
            </button>
          </div>
          <div className="space-y-6">
            {NEWS_ITEMS.map((news, idx) => (
              <div key={idx} className="group cursor-pointer border-b border-[#B8AFA6]/40 pb-6 last:border-0 last:pb-0">
                <p className="text-xs text-[#D4AF37] mb-2 font-medium tracking-wider">{news.date}</p>
                <h4 className="font-serif text-lg text-[#1A1A1A] group-hover:text-[#6B6B6B] transition-colors mb-2">{news.title}</h4>
                <p className="text-[#6B6B6B] text-sm line-clamp-2">{news.desc}</p>
              </div>
            ))}
          </div>
        </FadeIn>
      </div>
    </section>
  </main>
);

const InfographicPage = ({ data, setView }) => (
  <main className="bg-[#EDEAE6]">
    {/* Section A: Hero Header */}
    <section className="pt-32 pb-20 px-6 max-w-[1000px] mx-auto text-center border-b border-[#B8AFA6]/30">
      <FadeIn>
        <div className="w-16 h-16 bg-[#1A1A1A] text-[#D4AF37] rounded-2xl flex items-center justify-center mx-auto mb-8 shadow-lg">
          {data.icon}
        </div>
        <h1 className="font-serif text-4xl md:text-6xl text-[#1A1A1A] mb-6 leading-tight">{data.title}</h1>
        <p className="text-xl text-[#6B6B6B] font-serif italic">{data.heroSubtitle}</p>
      </FadeIn>
    </section>

    {/* Section B: Intro */}
    <section className="py-[100px] px-6 max-w-[1200px] mx-auto">
      <div className="grid grid-cols-1 md:grid-cols-2 gap-16 items-center">
        <FadeIn delay={100}>
          <h2 className="font-serif text-3xl text-[#1A1A1A] mb-6">The Concept</h2>
          <p className="text-[#6B6B6B] text-lg leading-relaxed">{data.introText}</p>
        </FadeIn>
        <FadeIn delay={200} className="relative h-[400px] bg-[#2F2F2F] rounded-[12px] border border-[#1A1A1A] overflow-hidden flex items-center justify-center">
          <div className="absolute inset-0 opacity-10 bg-[radial-gradient(circle_at_center,_var(--tw-gradient-stops))] from-[#D4AF37] to-transparent"></div>
          {/* Abstract geometric representation */}
          <div className="relative w-48 h-48 border border-[#D4AF37] rounded-full flex items-center justify-center animate-[spin_40s_linear_infinite]">
            <div className="absolute w-full h-[1px] bg-[#D4AF37]/50 rotate-45"></div>
            <div className="absolute w-full h-[1px] bg-[#D4AF37]/50 -rotate-45"></div>
            <div className="w-32 h-32 border border-[#B8AFA6] rounded-full"></div>
            <div className="w-16 h-16 bg-[#1A1A1A] rounded-full absolute flex items-center justify-center z-10">
               {data.icon}
            </div>
          </div>
        </FadeIn>
      </div>
    </section>

    {/* Section C: Process / Flow */}
    <section className="bg-[#1A1A1A] py-[100px] px-6">
      <div className="max-w-[1200px] mx-auto">
        <FadeIn>
          <h2 className="font-serif text-3xl text-[#EDEAE6] mb-16 text-center">The Workflow</h2>
        </FadeIn>
        <div className="flex flex-col md:flex-row justify-between items-center relative">
          {/* Connecting line for desktop */}
          <div className="hidden md:block absolute top-1/2 left-[10%] right-[10%] h-[1px] bg-[#2F2F2F] -translate-y-1/2 z-0"></div>
          
          {data.process.map((step, idx) => (
            <FadeIn delay={idx * 150} key={idx} className="relative z-10 flex flex-col items-center mb-8 md:mb-0 bg-[#1A1A1A] px-4">
              <div className="w-12 h-12 rounded-full border-2 border-[#D4AF37] text-[#D4AF37] flex items-center justify-center font-serif text-lg mb-4 bg-[#1A1A1A]">
                {idx + 1}
              </div>
              <p className="text-[#EDEAE6] font-medium text-center w-32">{step}</p>
            </FadeIn>
          ))}
        </div>
      </div>
    </section>

    {/* Section D: Key Stats */}
    <section className="py-[100px] px-6 max-w-[1200px] mx-auto border-b border-[#B8AFA6]/30">
      <div className="grid grid-cols-1 md:grid-cols-3 gap-12 text-center">
        {data.stats.map((stat, idx) => (
          <FadeIn delay={idx * 100} key={idx}>
            <p className="font-serif text-6xl md:text-7xl text-[#1A1A1A] mb-4">{stat.value}</p>
            <p className="text-[#6B6B6B] tracking-widest uppercase text-sm font-semibold">{stat.label}</p>
          </FadeIn>
        ))}
      </div>
    </section>

    {/* Section E: Visual Breakdown */}
    <section className="py-[100px] px-6 max-w-[1200px] mx-auto">
      <FadeIn>
        <h2 className="font-serif text-3xl text-[#1A1A1A] mb-16 text-center">Core Innovations</h2>
      </FadeIn>
      <div className="grid grid-cols-1 md:grid-cols-2 gap-x-12 gap-y-16">
        {data.features.map((feature, idx) => (
          <FadeIn delay={idx * 100} key={idx} className="flex gap-6">
            <div className="mt-1 flex-shrink-0 w-12 h-12 rounded-[10px] bg-[#EDEAE6] border border-[#B8AFA6] text-[#1A1A1A] flex items-center justify-center">
              {feature.icon}
            </div>
            <div>
              <h3 className="font-serif text-xl text-[#1A1A1A] mb-2">{feature.title}</h3>
              <p className="text-[#6B6B6B] leading-relaxed">{feature.desc}</p>
            </div>
          </FadeIn>
        ))}
      </div>
    </section>

    {/* Section F: CTA */}
    <section className="py-[100px] px-6 text-center bg-[#2F2F2F]">
      <FadeIn>
        <h2 className="font-serif text-4xl text-[#EDEAE6] mb-8">Ready to dive deeper?</h2>
        <div className="flex justify-center gap-6">
          <button 
            onClick={() => setView('home')}
            className="px-8 py-4 border border-[#B8AFA6] text-[#EDEAE6] rounded-[12px] hover:bg-[#EDEAE6] hover:text-[#1A1A1A] transition-colors"
          >
            Back to Home
          </button>
          <button 
            onClick={() => {
              const currentIndex = TOPICS.findIndex(t => t.id === data.id);
              const nextIndex = (currentIndex + 1) % TOPICS.length;
              setView(TOPICS[nextIndex].id);
              window.scrollTo(0,0);
            }}
            className="px-8 py-4 bg-[#D4AF37] text-[#1A1A1A] font-medium rounded-[12px] hover:bg-[#E5C254] transition-colors shadow-lg"
          >
            Explore Next Topic
          </button>
        </div>
      </FadeIn>
    </section>
  </main>
);

const MediaNewsPage = () => (
  <main className="pb-[100px]">
    {/* Header */}
    <section className="bg-[#1A1A1A] pt-32 pb-24 px-6 text-center">
      <FadeIn>
        <h1 className="font-serif text-5xl md:text-6xl text-[#EDEAE6] mb-6">Media & Insights</h1>
        <p className="text-[#B8AFA6] text-lg max-w-2xl mx-auto">
          Immerse yourself in the visual documentation of our latest breakthroughs, from deep-dive documentaries to rapid news bites.
        </p>
      </FadeIn>
    </section>

    {/* Video Grid */}
    <section className="py-[100px] px-6 max-w-[1200px] mx-auto border-b border-[#B8AFA6]/30">
      <FadeIn>
        <div className="flex items-center gap-3 mb-10">
          <FileVideo className="text-[#D4AF37]" size={24} />
          <h2 className="font-serif text-3xl text-[#1A1A1A]">Video Library</h2>
        </div>
      </FadeIn>
      <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
        {VIDEO_ITEMS.map((video, idx) => (
          <FadeIn delay={idx * 100} key={idx} className="group">
            <div className="w-full aspect-video bg-[#1A1A1A] rounded-[12px] relative overflow-hidden mb-4 border border-[#B8AFA6]/20 shadow-sm transition-all duration-300">
              <iframe 
                width="100%" 
                height="100%" 
                src={`https://www.youtube.com/embed/${video.youtubeId}?rel=0`}
                title={video.title}
                frameBorder="0" 
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                allowFullScreen
                className="absolute inset-0"
              ></iframe>
            </div>
            <h3 className="font-serif text-lg text-[#1A1A1A]">{video.title}</h3>
          </FadeIn>
        ))}
      </div>
    </section>

    {/* News Grid */}
    <section className="py-[100px] px-6 max-w-[1200px] mx-auto">
      <FadeIn>
        <div className="flex items-center gap-3 mb-10">
          <Newspaper className="text-[#D4AF37]" size={24} />
          <h2 className="font-serif text-3xl text-[#1A1A1A]">Latest News</h2>
        </div>
      </FadeIn>
      <div className="grid grid-cols-1 md:grid-cols-3 gap-8">
        {[...NEWS_ITEMS, ...NEWS_ITEMS].map((news, idx) => ( // Duplicating for grid fill effect
          <FadeIn delay={idx * 100} key={idx} className="bg-[#EDEAE6] border border-[#B8AFA6]/50 rounded-[12px] p-6 flex flex-col h-full hover:bg-white transition-colors hover:shadow-[0_10px_20px_rgba(0,0,0,0.03)] group">
            <div className="w-full h-40 bg-[#2F2F2F] rounded-[8px] mb-6 flex items-center justify-center opacity-90 group-hover:opacity-100 transition-opacity">
               <Activity size={32} className="text-[#B8AFA6]/30" />
            </div>
            <p className="text-xs text-[#D4AF37] mb-3 font-semibold tracking-wider uppercase">{news.date}</p>
            <h3 className="font-serif text-xl text-[#1A1A1A] mb-3">{news.title}</h3>
            <p className="text-[#6B6B6B] text-sm leading-relaxed mb-6 flex-grow">{news.desc}</p>
            <span className="text-[#1A1A1A] text-sm font-semibold flex items-center group-hover:text-[#D4AF37] transition-colors mt-auto">
              Read Article <ChevronRight size={16} className="ml-1 group-hover:translate-x-1 transition-transform" />
            </span>
          </FadeIn>
        ))}
      </div>
    </section>
  </main>
);

// --- MAIN APP COMPONENT ---

export default function App() {
  const [view, setView] = useState('home');

  // Scroll to top on view change
  useEffect(() => {
    window.scrollTo(0, 0);
  }, [view]);

  // Inject styles safely
  useEffect(() => {
    const styleSheet = document.createElement("style");
    styleSheet.innerText = styles;
    document.head.appendChild(styleSheet);
    return () => { document.head.removeChild(styleSheet); };
  }, []);

  const renderView = () => {
    if (view === 'home') return <HomePage setView={setView} />;
    if (view === 'media') return <MediaNewsPage />;
    
    // Check if view matches a topic ID
    const topicData = TOPICS.find(t => t.id === view);
    if (topicData) return <InfographicPage data={topicData} setView={setView} />;
    
    return <HomePage setView={setView} />; // Fallback
  };

  return (
    <div className="min-h-screen flex flex-col relative">
      <Navbar currentView={view} setView={setView} />
      <div className="flex-grow">
        {renderView()}
      </div>
      <Footer />
    </div>
  );
}