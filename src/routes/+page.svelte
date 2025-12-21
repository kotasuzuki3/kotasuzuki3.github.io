<script>
  import Caret from "$lib/blinkingCaret.svelte";
  import Card from "$lib/Card.svelte";
</script>

<div class="snap-y snap-mandatory">
  <section id="hero" class="container mx-auto flex flex-col justify-center min-h-screen relative">
    <div class="flex flex-col md:flex-row md:items-start">
      <div class="flex flex-row mx-5 justify-center md:justify-start">
        <h1 class="text-6xl font-medium md:text-8xl lg:whitespace-nowrap">&gt;Hello World.</h1>
        <Caret />
      </div>
      <div class="post-it relative md:-translate-y-12">
      <div class="items-center md:text-md mx-14 md:ml-5 mt-3 md:mt-0 xl:text-lg">
        <p>
          My name is
          <a
            href="https://www.linkedin.com/in/kota-suzuki-77107324b/"
            target="_blank"
            rel="noreferrer"
            class="underline hover:bg-blue-500 cursor-pointer transition duration-300"
          >
            Kota Suzuki.
          </a>
        </p>
        <p>I am a data analyst with a multimedia journalism background.</p>
        <p>
          I studied journalism, data science, and statistics at
          <a
            href="https://www.northwestern.edu/"
            target="_blank"
            rel="noreferrer"
            class="underline hover:bg-blue-300 cursor-pointer transition duration-300"
          >
            Northwestern University.
          </a>
        </p>
      </div>
      </div>
    </div>

  <div class="contacts grid grid-flow-col auto-cols-max gap-4 justify-center md:justify-start md:ml-5 md:-translate-y-22">
      <a href="mailto: kotasuzuki2025@alum.northwestern.edu">
        <img src="/email.png" alt="Email" class="size-9" />
      </a>
      <h1 class="text-3xl">|</h1>

      <a href="https://www.linkedin.com/in/kota-suzuki-77107324b/" target="_blank" rel="noreferrer">
        <img src="/linkedin.png" alt="LinkedIn" class="size-7 translate-y-[2px]" />
      </a>
      <h1 class="text-3xl">|</h1>

      <a href="https://github.com/kotasuzuki3" target="_blank" rel="noreferrer">
        <img src="/github.png" alt="GitHub" class="size-9 -translate-y-[2px]" />
      </a>
    </div>

    <div id="navigation-arrow" class="self-center absolute bottom-0 mb-12 animate-bounce">
      <a href="#projects" aria-label="Jump to projects">
        <svg class="w-14 h-14" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor">
          <path stroke-linecap="round" stroke-linejoin="round" d="m9 12.75 3 3m0 0 3-3m-3 3v-7.5M21 12a9 9 0 1 1-18 0 9 9 0 0 1 18 0Z" />
        </svg>
      </a>
    </div>
  </section>

  <section id="projects" class="min-h-screen container mx-auto px-6 py-16">
    <h2 class="projects-title">Projects</h2>
    <div class="projects-grid">
        <Card title="SAY THEIR NAMES Project" img_path="/projects/STN.png" summary="I built an interactive map with filters and time controls to explore incident-level, police violence data across the U.S." link="https://nonopera.dreamhosters.com/voices/say-their-names/" tools={["React", "Leaflet", "SQL"]}/>
        <Card title="San Francisco Chronicle 2024 Election" img_path="/projects/SFChron.png" summary="I built custom data visualizations and automated data pipelines for the Chronicle's first-ever, nine-county Bay Area election coverage." link="https://www.sfchronicle.com/projects/2024/election-results/san-francisco" tools={["Datawrapper", "d3.js", "Pandas", "Python", "geocoding"]}/>
        <Card title="The Daily Northwestern Annual Poll" img_path="/projects/NUpoll.png" summary="How did Northwestern students feel about the encampment? What are students' life habits? We found out through The Daily's first-ever annual poll." link="https://dailynorthwestern.com/2024/10/23/campus/f24-poll/" tools={["Datawrapper", "Python", "BeautifulSoup"]}/>
        <Card title="Survey and Intervention Chatbot" img_path="/projects/DSI.png" summary="Can you replace door-to-door deep canvassing with a chatbot? I tried to answer this question by building a modular chatbot with randomization, video/image, and AI functionality." link="https://datascience.uchicago.edu/people/kota-suzuki/" tools={["Python", "WhatsApp API", "OpenAI API","PostgreSQL"]}/>
        <Card title="Gut Microbiome Research" img_path="/projects/gutmicrobiome.png" summary="I led the data cleaning and EDA efforts on a comprehensive, 17,000-sample gut microbiome dataset to further microbial meta-analysis efforts." link="https://www.poopomics.com/publications" tools={["Python", "R", "Pandas","ggplot"]}/>
    </div>
  </section>
</div>
