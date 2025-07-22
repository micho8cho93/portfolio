<script lang="ts">
  export let activeSection: string;
  import { Mail } from "lucide-svelte";
  import { Linkedin } from "lucide-svelte";
  import { Github } from "lucide-svelte";
</script>


<header
  class="lg:sticky lg:top-0 lg:flex lg:max-h-screen lg:w-1/2 lg:flex-col lg:justify-around "
>
  <div>
    <h1 class="text-4xl font-bold tracking-tight text-slate-200 sm:text-5xl">
      Michel Honoré
    </h1>
    
    <p class="mt-4 max-w-m leading-normal">
      Computer Science Teacher & Software Tinkerer
    </p>
    <!-- Navigation -->
    <nav class="nav hidden lg:block" aria-label="In-page jump links">
      <ul class="mt-8 w-max">
        <li>
          <a
            class="group flex items-center py-3 active"
            href="#about"
            
          >
            <span
              class="nav-indicator mr-4 h-px transition-all
                group-hover:w-16 group-hover:bg-slate-200
                motion-reduce:transition-none
                {activeSection === 'about' ? 'w-16 bg-slate-200' : 'w-8 bg-slate-600'}"
            ></span>
            <span
              class="nav-text text-xs font-bold uppercase tracking-widest
                group-hover:text-slate-200
                {activeSection === 'about' ? 'text-slate-200' : 'text-slate-500'}"
            >
              About
            </span>
          </a>
        </li>
        <li>
          <a class="group flex items-center py-3" href="#experience">
            <span
              class="nav-indicator mr-4 h-px transition-all
                group-hover:w-16 group-hover:bg-slate-200
                motion-reduce:transition-none
                {activeSection === 'experience' ? 'w-16 bg-slate-200' : 'w-8 bg-slate-600'}"
            ></span>
            <span
              class="nav-text text-xs font-bold uppercase tracking-widest
                group-hover:text-slate-200
                {activeSection === 'experience' ? 'text-slate-200' : 'text-slate-500'}"
            >
              Experience
            </span>
          </a>
        </li>
        <li>
          <a class="group flex items-center py-3" href="#projects">
            <span
              class="nav-indicator mr-4 h-px transition-all
                group-hover:w-16 group-hover:bg-slate-200
                motion-reduce:transition-none
                {activeSection === 'projects' ? 'w-16 bg-slate-200' : 'w-8 bg-slate-600'}"
            ></span>
            <span
              class="nav-text text-xs font-bold uppercase tracking-widest
                group-hover:text-slate-200
                {activeSection === 'projects' ? 'text-slate-200' : 'text-slate-500'}"
            >
              Projects
            </span>
          </a>
        </li>
      </ul>
    </nav>
    <br>

<!-- Skills -->
    <section class="nav hidden lg:block" aria-label="skillset">
      <span
              class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200"
            >
              Programming Languages
            </span>
      <ul class="mt-2 flex flex-wrap space-x-1 space-y-1 w-50">
        <li>
            
            <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Python
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  JavaScript
                </div>
        </li>
        <li>
            <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Arduino/C++
                </div>
        </li>
        <li>
            <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  HTML
                </div>
        </li>
        <li>
            <div
                  class="flex items-center rounded-full bg-teal-400/10 px-3 py-1 text-xs font-medium leading-5 text-teal-300"
                >
                  Tailwind/CSS
                </div>
        </li>
        </ul>
        <br>

        <span
              class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200"
            >
              Frameworks & Tools
            </span>
        <ul class="mt-2 flex flex-wrap space-x-1 space-y-1 w-50">
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Git
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  GitHub
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Streamlit
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Django
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Vercel
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Railway
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  SQLite
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  PostgreSQL
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Crontab
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-blue-400/10 px-3 py-1 text-xs font-medium leading-5 text-blue-300"
                >
                  Gemini CLI
                </div>
        </li>
        </ul>
        <br>

        <span
              class="nav-text text-xs font-bold uppercase tracking-widest text-slate-500 group-hover:text-slate-200 group-focus-visible:text-slate-200"
            >
              Education
            </span>
        <ul class="mt-2 flex flex-wrap space-x-1 space-y-1 w-50">
        <li>
            
            <div
                  class="flex items-center rounded-full bg-fuchsia-400/10 px-3 py-1 text-xs font-medium leading-5 text-fuchsia-300"
                >
                  CS Principles
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-fuchsia-400/10 px-3 py-1 text-xs font-medium leading-5 text-fuchsia-300"
                >
                  Project-based Learning
                </div>
        </li>
        <li>
            
            <div
                  class="flex items-center rounded-full bg-fuchsia-400/10 px-3 py-1 text-xs font-medium leading-5 text-fuchsia-300"
                >
                  Robotics
                </div>
        </li>
      </ul>
    </section>
  


  <!-- Social Links -->
      <ul class="ml-1 mt-8 flex items-center" aria-label="Social media">
        <li class="mr-5 text-xs">
          <a
            class="block hover:text-slate-100"
            href="https://github.com/micho8cho93"
            target="_blank"
            rel="noreferrer"
          >
            <Github class="h-6 w-6" />
          </a>
        </li>
        <li class="mr-5 text-xs">
          <a
            class="block hover:text-slate-100"
            href="https://www.linkedin.com/in/michel-honore-95a08549/"
            target="_blank"
            rel="noreferrer"
          >
            <Linkedin class="h-6 w-6" />
          </a>
        </li>
        <li class="mr-5 text-xs">
          <a
            class="block hover:text-slate-100"
            href="mailto:michelvahonore@gmail.com"
            target="_blank"
            rel="noreferrer"
          >
            <Mail class="h-6 w-6" />
          </a>
        </li>
      </ul>
    
  </div>
</header>

