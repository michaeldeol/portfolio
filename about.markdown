---
layout: about
title: About
permalink: /about/
---

<div class="min-h-screen bg-gradient-to-br from-slate-900 via-slate-800 to-slate-900 py-20">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    
    <!-- Hero Section -->
    <div class="text-center mb-16">
      <div class="w-32 h-32 mx-auto mb-8 rounded-full overflow-hidden shadow-xl ring-4 ring-white/10 hover:ring-white/20 transition-all duration-300">
        <!-- Replace this URL with your actual avatar image -->
        <img src="{{ '/assets/images/25035.jpg' | relative_url }}" 
             alt="Michael Deol" 
             class="w-full h-full object-cover hover:scale-105 transition-transform duration-300">
      </div>
      <h1 class="text-4xl md:text-5xl font-bold text-white mb-6">About Me</h1>
      <p class="text-xl text-slate-300 max-w-2xl mx-auto">
        Passionate developer with a love for creating beautiful, functional, and user-friendly applications.
      </p>
    </div>

    <!-- Main Content -->
    <div class="bg-slate-800 border border-slate-700 rounded-2xl shadow-2xl p-8 md:p-12 mb-12">
      <div class="prose prose-lg max-w-none">
        <h2 class="text-3xl font-bold text-white mb-6">My Journey</h2>
        <p class="text-slate-300 mb-6">
          My journey into software began in the late '90s, when I taught myself how to build websites to showcase the classic car shows I loved attending. Armed with a digital camera and a passion for hot rods and customs, I wanted to share our local scene with the rest of the world. That early blend of storytelling and technology sparked a lifelong obsession with building things that connect people.
        </p>
        
        <p class="text-slate-300 mb-6">
          Over the years, I took on contract work across industries—refining my skills in backend architecture, cloud infrastructure, and full-stack development. My professional break came at Overstock.com, where I founded and scaled the frontend engineering team, leading accessibility and performance initiatives while staying hands-on with the code.
        </p>
        
        <p class="text-slate-300 mb-6">
          From there, I dove deep into the startup world—building scalable systems at Acorns and leading engineering at Blast, where speed, iteration, and impact were daily rhythms. I've since architected cloud services at Oracle and mentored teams while continuing to ship production code.
        </p>
        
        <p class="text-slate-300 mb-6">
          Through it all, I've remained a builder at heart—driven by curiosity, collaboration, and the joy of turning complex problems into elegant, intuitive solutions.
        </p>        <h3 class="text-2xl font-bold text-white mb-4">What I Do</h3>
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 mb-8">
          <div class="bg-indigo-900/30 border border-indigo-500/30 rounded-lg p-6 hover:border-indigo-400/50 transition-colors duration-200">
            <h4 class="text-lg font-semibold text-indigo-400 mb-3">Frontend Development</h4>
            <p class="text-slate-300">Creating responsive, interactive user interfaces with modern frameworks and libraries.</p>
          </div>
          <div class="bg-emerald-900/30 border border-emerald-500/30 rounded-lg p-6 hover:border-emerald-400/50 transition-colors duration-200">
            <h4 class="text-lg font-semibold text-emerald-400 mb-3">Backend Development</h4>
            <p class="text-slate-300">Building robust server-side applications and APIs that power great user experiences.</p>
          </div>
          <div class="bg-purple-900/30 border border-purple-500/30 rounded-lg p-6 hover:border-purple-400/50 transition-colors duration-200">
            <h4 class="text-lg font-semibold text-purple-400 mb-3">Full-Stack Solutions</h4>
            <p class="text-slate-300">Connecting frontend and backend technologies to deliver complete web applications.</p>
          </div>
          <div class="bg-orange-900/30 border border-orange-500/30 rounded-lg p-6 hover:border-orange-400/50 transition-colors duration-200">
            <h4 class="text-lg font-semibold text-orange-400 mb-3">Problem Solving</h4>
            <p class="text-slate-300">Analyzing complex requirements and delivering elegant, efficient solutions.</p>
          </div>
        </div>

        <h3 class="text-2xl font-bold text-white mb-4">Technologies & Tools</h3>
        <p class="text-slate-300 mb-6">
          I work with a variety of technologies to bring ideas to life. Here are some of my favorites:
        </p>
        
        {% include technologies.html %}
      </div>
    </div>

    <!-- Contact CTA -->
    <div class="bg-gradient-to-r from-indigo-600 via-purple-600 to-pink-600 rounded-2xl p-8 md:p-12 text-center text-white shadow-2xl">
      <h2 class="text-3xl font-bold mb-4">Let's Connect</h2>
      <p class="text-indigo-100 mb-8 text-lg">
        I'm always interested in new opportunities and exciting projects.
      </p>
      <div class="flex flex-col sm:flex-row gap-4 justify-center">
        <a href="mailto:{{ site.email }}" class="bg-white text-indigo-600 px-8 py-3 rounded-lg font-semibold hover:bg-slate-100 hover:shadow-lg transition-all duration-200 transform hover:-translate-y-0.5">
          Send me an email
        </a>
        {% if site.github_username %}
        <a href="https://github.com/{{ site.github_username }}" class="border-2 border-white text-white px-8 py-3 rounded-lg font-semibold hover:bg-white hover:text-indigo-600 transition-all duration-200 transform hover:-translate-y-0.5">
          Check out my GitHub
        </a>
        {% endif %}
      </div>
    </div>
    
  </div>
</div>
