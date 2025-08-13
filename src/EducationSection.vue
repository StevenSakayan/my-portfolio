<script setup>
import Window from './WindowContainer.vue';
import EducationSubList from './EducationSubList.vue'


</script>

<template>
    <Window title="Education.pdf">
      <div class="px-10 py-10 max-sm:px-5">
        <div class="flex">
          <a href="https://www.csu.edu.au/" target="_blank" class="flex w-40 max-sm:w-20 h-40 max-sm:h-20 bg-white rounded-full items-center justify-center">
            <img class= "w-30 h-30 max-sm:w-15 max-sm:h-15 object-contain transition duration-200 ease-in-out hover:scale-110" src="/images/csu.png"/>
          </a>
          <div class="flex flex-col h-fit self-center ml-5">
            <h1 class="text-2xl font-bold">Bachelor of Information Technology</h1>
            <h1 class="text-xl">Specialisation in Software Development</h1>
            <h2 class="text-lg italic"><a href="https://www.csu.edu.au/" target="_blank" class="link">Charles Sturt University</a> | 2023 - Present</h2>
            <h2 class="font-bold">Current GPA: 5.59</h2>
          </div>
        </div>
        <h1 class="text-2xl mt-5 font-bold">Studied Topics</h1>
        <div class="flex">
          <ul class="list-disc list-inside font-bold mt-5">
            <li class="pb-3">Programming Principles
              <EducationSubList>
                <li>Problem Solving</li>
                <li>Error Debugging</li>
                <li>Interpreting & Writing Algorithms</li>
                <li>Analysis, Design, Coding, Testing, & Documentation</li>
              </EducationSubList>
            </li>
            <li class="pb-3">Introduction to the Web
              <EducationSubList>
                <li>Web & Webpage Anatomy</li>
                <li>HTML</li>
                <li>CSS</li>
                <li>JavaScript</li>
              </EducationSubList>
            </li>
            <li class="pb-3">Data Structures
              <EducationSubList>
                <li>Design Patterns for Data Structures</li>
                <li>Linear & Binary Search</li>
                <li>ArrayLists</li>
                <li>Linked Data Representations</li>
                <li>Recursive Functions</li>
                <li>Stacks, Queues, Binary Trees, Heaps, & Graphs</li>
                <li>Sorting, Big-O Notation, & Sort Comparisons</li>
              </EducationSubList>
            </li>
          </ul>
          <div class="divider divider-horizontal"></div>
          <ul class="list-disc list-inside font-bold mt-5">
            <li class="pb-3">Programming in Java 1 + 2
              <EducationSubList>
                <li>Object-Based Programming</li>
                <li>UML to Design Requirements</li>
                <li>Class Design & Implementation</li>
                <li>Testing & Debugging Techniques</li>
                <li>Inheritance: Base, Derived, & Abstract</li>
                <li>Collection Data Structures</li>
                <li>Application Development</li>
                <li>File Manipulation</li>
                <li>GUI Programming & Graphics</li>
                <li>Event-Driven Programming</li>
                <li>Read & Write SQL Database</li>
                <li>Threads</li>
              </EducationSubList>
            </li>
            <li class="pb-3">Human Computer Interaction
              <EducationSubList>
                <li>Capturing User Requirements</li>
                <li>UI Principles</li>
                <li>UI Ergonomics</li>
              </EducationSubList>
            </li>
            <li class="pb-3">Database Systems
              <EducationSubList>
                <li>Databases & DMS</li>
                <li>Relational Database Model</li>
                <li>Entity Relationship Diagrams</li>
                <li>Normalisation</li>
                <li>Implementation through SQL</li>
                <li>Querying through SQL</li>
                <li>Security</li>
              </EducationSubList>
            </li>
          </ul>
        </div>
        <div class="divider divider-vertical"></div>
        <h1 class="text-2xl mt-10 font-bold">Awards</h1>

        <a class="font-bold link" href="./documents/2023 Executive Dean's Award-1.pdf" target="_blank">🏅 Executive Dean's Award - 2023</a>
        <h3 class="mb-5">Professor Lewis Bizo - Charles Sturt University</h3>

        <a class="font-bold link" href="./documents/2024 Executive Dean's Award-1.pdf" target="_blank">🏅 Executive Dean's Award - 2024</a>
        <h3 class="">Professor Lewis Bizo - Charles Sturt University</h3>
      </div>
    </Window>
</template>
