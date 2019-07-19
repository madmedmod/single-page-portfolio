<template>
  <div class="container">
    <div>
      <NavbarSection />
      <WelcomeSection />
      <ProjectsSection />
      <ContactSection />
      <FooterSection />
    </div>
  </div>
</template>

<script>
import NavbarSection from '~/components/NavbarSection.vue'
import WelcomeSection from '~/components/WelcomeSection.vue'
import ProjectsSection from '~/components/ProjectsSection.vue'
import ContactSection from '~/components/ContactSection.vue'
import FooterSection from '~/components/FooterSection.vue'

export default {
  components: {
    NavbarSection,
    WelcomeSection,
    ProjectsSection,
    ContactSection,
    FooterSection
  }
}
</script>

<style lang="sass">
@import url('https://fonts.googleapis.com/css?family=DM+Sans|Lato|Montserrat|Roboto&display=swap');
/* custom variables */
$body-color: #f8f8f8 // all font colors
$nav-color: #00b8a9 // navbar
$nav-list-color: #45969b // nav hover and projects bg colors + footer list
$project-bg-color: #113f67 //specific project bg, contact and footer colors
//
// white : #f8f8f8
// blue 2 : #45969b
// navy blue : #085f63
// navy 2 : #113f67
// blue 22 : #226597
// soft blue : #87c0cd
// 2nd blue : $49beb7

/* Mixin media query setups */
/* 1200px / 16px = 75em */
@mixin for-desktop
  @media (max-width: 75em){ @content; }

/* 980px / 16px = 61.25em */
@mixin for-tablet
  @media (max-width: 62.25em){ @content; }

/* 460px / 16px = 28.75em */
@mixin for-phone
  @media (max-width: 28.75em){ @content; }

  /* "Automagic" image grid using no media  */
@mixin auto-magic
  @media (max-width: 30.625em){ @content; }
*
  margin: 0
  padding: 0
  &:before, &:after
    box-sizing: inherit

html
  box-sizing: border-box
  /*  */
  font-size: 62.5%
  scroll-behavior: smooth
  @include for-desktop
    font-size: 60%
  @include for-tablet
    font-size: 58%
  @include for-phone
    font-size: 55%

body
  font-family: 'Lato',sans-serif
  font-size: 1.8rem
  font-weight: 400
  line-height: 1.4
  color: $body-color

h1,h2
  font-family: 'Lato',sans-serif
  font-weight: 700
  text-align: center

h1
  font-size: 6rem

h2
  font-size: 4.2rem

ul
  list-style: none
a
  text-decoration: none
  color: $body-color

img
  display: block
  width: 100%

/* nav */
.nav
  display: flex
  justify-content: flex-end
  position: fixed
  top: 0
  left: 0
  width: 100%
  background: $nav-color
  box-shadow: 0 2px 0 rgba(0, 0, 0, 0.4)
  z-index: 10
  @include for-phone
    justify-content: center

.nav-list
  display: flex
  margin-right: 2rem
  @include for-phone
    margin: 0 1rem
  a
    display: block
    font-size: 2.2rem
    padding: 2rem
    &:hover
      background: $nav-list-color

/* welcome section */
.welcome-section
  display: flex
  flex-direction: column
  justify-content: center
  align-items: center
  width: 100%
  height: 100vh
  background-color: $project-bg-color
  // background-image: linear-gradient(62deg, #222831 0%, #393e46 100%)
  > p
    font-size: 3rem
    font-weight: 200
    font-style: italic
    color: $nav-color

/* Projects section */

.projects-section
  text-align: center
  padding: 10rem 2rem
  background: $nav-list-color
  @include auto-magic
    padding: 6rem 1rem

.projects-section-header
  max-width: 420px
  margin: 0 auto 6rem auto
  border-bottom: 0.2rem solid $project-bg-color
  @include for-phone
    font-size: 4rem

.projects-grid
  display: grid
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr))
  grid-gap: 4rem
  width: 100%
  max-width: 1280px;
  margin: 0 auto
  margin-bottom: 6rem
  @include auto-magic
    grid-template-columns: 1fr

.project
  background: $project-bg-color
  box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5)
  border-radius: 2px

  &:hover .code
    color: #ff7f50

.code
  color: $project-bg-color
  transition: color 0.3s ease-out

.project-image
  height: calc(100% - 6.8rem)
  width: 100%
  object-fit: cover

.project-title
  font-size: 2rem
  padding: 2rem 0.5rem

.btn
  display: inline-block
  padding: 1rem 2rem
  border-radius: 2px

.btn-show-all
  font-size: 2rem
  background: $project-bg-color
  transition: background 0.3s ease-out
  &:hover
    background: $nav-color
    > i
    margin-left: 10px
    transform: translateX(0)
    transition: transform 0.3s ease-out

/* contact section */
.contact-section
  display: flex
  flex-direction: column
  justify-content: center
  align-items: center
  text-align: center
  width: 100%
  height: 80vh
  padding: 0 2rem
  background: $project-bg-color

.contact-section-header
  > h2
    font-size: 6rem
    @include for-phone
      font-size: 4rem
  > p
    font-style: italic

.contact-links
  display: flex
  justify-content: center
  width: 100%
  max-width: 980px
  margin-top: 4rem
  flex-wrap: wrap

.contact-details
  font-size: 2.4rem
  text-shadow: 2px 2px 1px #1f1f1f
  transition: transform 0.3s ease-out

  &:hover
    transform: translateY(8px)

/* Footer */
footer
  font-weight: 300
  display: flex
  justify-content: space-evenly
  padding: 2rem
  background: $project-bg-color
  border-top: 4px solid $nav-color
  @include for-phone
    flex-direction: column
    text-align: center
  > p
    margin: 2rem
  i
    vertical-align: middle
</style>
