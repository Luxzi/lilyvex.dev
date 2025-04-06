<template>
  <UApp>
    <div class="flex h-screen p-4">
      <div class="m-auto max-w-2xl">
        <div class="text-center">
          <h1 class="text-6xl inline-flex">Hi! I'm <p class="font-bold ml-6">Lily</p></h1>
        </div>
        <div class="text-center mt-3">
          <p class="mono">Lily Vex (she/her) <<NuxtLink to="https://github.com/Luxzi.gpg" class="link cursor-pointer">PGP</NuxtLink>></p>
        </div>
        <div class="flex justify-center mt-5">
          <Button class="mr-2" ><NuxtLink to="https://github.com/Luxzi/" class="cursor-pointer flex">View projects <Icon name="material-symbols-light:arrow-circle-right-rounded" size="1.5em" class="ml-2" /></NuxtLink></Button>
          <Button variant="secondary"><NuxtLink to="mailto:contact@lilyvex.dev" class="cursor-pointer flex">Contact <Icon name="material-symbols-light:mail" size="1.5em" class="ml-2" /></NuxtLink></Button>
        </div>

        <br>
        <hr class="fill-amber-300">
        <!-- <h3 class="roles text-center p-3 font-bold">Software Engineer & Security Researcher</h3> -->
        <br>
        
        <h2 class="font-bold text-2xl mb-4">About me & my work</h2>
        <p>
          I do systems programming with <Technology label="Rust" icon="cib:rust" link="https://rust-lang.org/" />, <Technology label="Go" icon="cib:go" link="https://golang.org/" />, 
          <Technology label="C++" icon="cib:cplusplus" link="https://en.wikipedia.org/wiki/C%2B%2B" />, and <Technology label="C" icon="cib:c" link="https://en.wikipedia.org/wiki/C_(programming_language)" />.
          I'm also familar with various scripting languages, operating systems,
          containerization technologies, and version control systems including,
          but not limited to, <Technology label="Python" icon="cib:python" link="https://python.org/" />,
          <Technology label="Ruby" icon="cib:ruby" link="https://www.ruby-lang.org/en/" />, <Technology label="Git" icon="cib:git" link="https://git-scm.org/" />, 
          <Technology label="Linux" icon="cib:linux" link="https://kernel.org/" />, <Technology label="Docker" icon="cib:docker" link="https://docker.com/" />,
          <Technology label="Kubernetes" icon="cib:kubernetes" link="https://kubernetes.io/" />, and many—many more.<br><br>

          I started programming in 2016, so around <NuxtTime class="rel-date" :datetime="new Date('2016-01-01T00:00:00')" relative />. I've always
          been interested in technology—computers specifically—and how it
          can be used to improve the lives of others.<br><br>

          Trans rights are human rights 🏳️‍⚧️<br><br>
        </p>
        <hr>
        <br>

        <div class="flex gap-10 justify-center">
          <Social icon="cib:github" link="https://github.com/Luxzi" alt="GitHub" />
          <Social icon="mdi:coffee" link="https://ko-fi.com/luxzi" alt="Kofi" size="2.35em" />
        </div><br>
        
        <hr>
        <br>

        <div class="flex justify-center">
          <h2 class="font-bold text-2xl mb-4">Cryptowallets</h2>
        </div>

        <div class="flex justify-center">
          <Wallet name="Monero" icon="cib:monero" address="87TuD9iKR9XdMjWyoMTZDqjLJWsu8bQqZUxM66EHhnR1JbuTUUcugApYQbnVAj7nhBDmcPr22h2kzHSfjLRpN13eLi8bPaR" />
        </div>
      </div>
    </div>
  </UApp>
</template>

<style scoped>
h1, h2, h3, p, span {
  font-family: "Inter", sans-serif;
}

Button {
  font-family: "Kode Mono", monospace;
}

.rel-date {
  font-family: "Kode Mono", monospace;
  background-color: rgb(70,70,70);
  padding: 4px;
  border-radius: 10px;
}

.mono {
  font-family: "Kode Mono", monospace;
}

.mono .link {
  display: inline;
  text-decoration: underline;
  text-decoration-thickness: .05em;
}

.roles {
  font-family: "Kode Mono", monospace;
}
</style>

<script lang="ts" setup>
  import Technology from '~/components/technology.vue';
</script>