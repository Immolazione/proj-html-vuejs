<template>
<div>
  <CoursesSection />
  <FacultiesSection />
  <AcademicYear :coachingSessions="coachingSessions" />
  <LatestCourses :latestCourses="latestCourses" :methodsAndFees="methodsAndFees" />
  <Subscribe />
  <Partners :partners="partners" />
</div>
</template>

<script>
import CoursesSection from './CoursesSection.vue'
import FacultiesSection from './FacultiesSection.vue'
import AcademicYear from './AcademicYear.vue'
import LatestCourses from './LatestCourses.vue'
import Subscribe from './Subscribe.vue'
import Partners from './Partners.vue'

export default {
  name: 'Main',
  components: {
    CoursesSection,
    FacultiesSection,
    AcademicYear,
    LatestCourses,
    Subscribe,
    Partners
  },
  data() {
    return {
      partners: [
        {image: 'partner-2.png', alt: 'medals'},
        {image: 'partner-3.png', alt: 'bulb'},
        {image: 'partner-4.png', alt: 'books'},
        {image: 'partner-5.png', alt: 'school-building'},
        {image: 'partner-6.png', alt: 'handmade'},
        {image: 'partner-8.png', alt: 'trophy'},
        {image: 'partner-1.png', alt: 'paperplane'},
        {image: 'partner-7.png', alt: 'communicating'},
      ],
      coachingSessions: [
        {title:'Coaching Session', 
        date: '20 May 21:30 PM', 
        description: 'Lorem, ipsum dolor sit amet consectetur adipisicing [...]'},

        {title:'Coaching Session', 
        date: '24 Mar 18:00 PM', 
        description: 'Lorem, ipsum dolor sit amet consectetur adipisicing [...]'},

        {title:'Coaching Session', 
        date: ' 12 Feb 13:30 PM', 
        description: 'Lorem, ipsum dolor sit amet consectetur adipisicing [...]'},

      ],

      latestCourses: [
        {image: 'Decisions-icon.png', title: 'Make Better Decisions', teacher: 'James Colins', price: '$21.00'},
        {image: 'Speaker-icon.png', title: 'How to be a speaker', teacher: 'James Colins', price: 'Free'},
        {image: 'Network-icon.png', title: 'Network Introductions', teacher: 'James Colins', price: 'Free'},
        {image: 'Brand-icon.png', title: 'Brand Management', teacher: 'James Colins', price: 'Free'}
      ],

      methodsAndFees: [
        {icon:'Exam-icon.png',
        image: 'Exam-Illustration.png', 
        title: 'The most efficient examination method', 
        paragraph: 'Eduprime has gathered teachers from around the globe to brainstorm in order to facilitate the evaluation of our students. Every teacher from our university has an influence on how students are evaluated at his/her subject.', 
        button: 'Discover the method',
        rowReverse: false},

        {icon: 'Exam-icon-1.png',
        image: 'Girl-Illustration.png', 
        title: 'Variable fees for international students', 
        paragraph: 'Eduprime has gathered teachers from around the globe to brainstorm in order to facilitate the evaluation of our students. Every teacher from our university has an influence on how students are evaluated at his/her subject.', 
        button: 'List of Fees',
        rowReverse: true}

      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import '../assets/scss/style.scss';
</style>
