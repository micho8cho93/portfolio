<script lang="ts">
  import { onMount } from "svelte";
  import Header from "$lib/components/Header.svelte";
  import About from "$lib/components/About.svelte";
  import Experience from "$lib/components/Experience.svelte";
  import Projects from "$lib/components/Projects.svelte";

  let activeSection = "about";

  const sections = ['about', 'experience', 'projects'];

  onMount(() => {
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          activeSection = entry.target.id;
        }
      });
    },
    { threshold: 0.6 });

    sections.forEach((id) => {
      const el = document.getElementById(id);
      if (el) observer.observe(el);
    });

    return () => observer.disconnect();
  })

</script>

<svelte:head>
  <script src="https://unpkg.com/@lottiefiles/dotlottie-wc@0.6.2/dist/dotlottie-wc.js" type="module"></script>
</svelte:head>


<div class="min-h-screen bg-indigo-950 text-slate-300">
  <dotlottie-wc 
  src="https://lottie.host/e17807d2-e628-4986-8a98-6043d39e97a6/J8KmsTE5H1.lottie" 
  style="width: 150px; height: 150px; position: fixed" 
  speed="1" 
  autoplay 
  loop
  ></dotlottie-wc>
  <div
    class="mx-auto max-w-screen-xl px-6 py-12 font-mono md:px-12 md:py-20 lg:px-24 lg:py-0"
  >
    <div class="lg:flex lg:justify-between lg:gap-4">
      <Header {activeSection} />
      <main class="pt-24 lg:w-1/2 lg:py-24">
        <About />
        <Experience />
        <Projects />
      </main>
    </div>
  </div>
</div>