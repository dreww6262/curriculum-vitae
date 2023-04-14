<script setup lang="ts">
import WelcomeItem from './WelcomeItem.vue'
import Icon from './Icon.vue'
</script>

<template>
  <div class="welcomeContainer">
  <WelcomeItem>
    <template #icon>
      <Icon imgName="reprise.avif" />
    </template>
    <template #heading>
      <a href="http://www.reprise.com" target="_blank" rel="noopener">Reprise</a></template
    >
    <p>Feb 2022 - Jan 2023 | Full Stack Engineer</p>
    <ul>
      <li>Implemented full stack features on the company's flagship Demo Editor</li>
      <li>Optimized data models and backend processes</li>
      <li>Created queries to tell meaningful stories through our analytics subsystem</li>
    </ul>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <Icon imgName="apokoz.jpg" />
    </template>
    <template #heading
      ><a href="https://github.com/akinpoz/akinpoz-mvp" target="_blank" rel="noopener"
        >Apokoz</a
      ></template
    >

    <p>May 2021 - Dec 2021 | Founder & Chief Product Officer</p>
    <ul>
      <li>Designed the first application to bring in novel revenue streams for restaurants.</li>
      <li>Implemented a full-stack MVP in React.js, Node.js, Javascript, AWS, CSS, and HTML.</li>
      <li>Made it to the final round of the &#x27;On Deck X&#x27; accelerator.</li>
    </ul>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <Icon imgName="bio.jpg" />
    </template>
    <template #heading
      ><a href="https://github.com/dreww6262/Bio" target="_blank" rel="noopener">Bio</a></template
    >

    <p>May 2020 - May 2021 | Founder & Chief Technical Officer</p>
    <ul>
      <li>
        Created a product geared towards self starters and influencers to promote their brand.
      </li>
      <li>Implemented a full stack MVP using Swift, Kotlin, and Google Cloud Platform.</li>
    </ul>
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <Icon imgName="booz_allen.jpg" />
    </template>
    <template #heading
      ><a
        href="https://www.boozallen.com/expertise/products/cybersecurity-products/district-defend.html"
        target="_blank"
        rel="noopener"
        >Booz Allen | District Defend</a
      ></template
    >

    <p>May 2019 - Aug 2019 | Software Development Intern</p>
    <ul>
      <li>
        Worked in an Agile workflow to create production components using AngularDart on top of a
        .NET Core framework.
      </li>
    </ul>
  </WelcomeItem>
  </div>
</template>

<style scoped lang="scss">
.welcomeContainer {
  margin: 0 auto;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  overflow-y: auto;
  padding-left: 30px;
}
</style>
