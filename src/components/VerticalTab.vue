<template>
    <div>
      <q-splitter
        v-model="splitterModel"
        style="height: 500px"
      >
  
        <template v-slot:before>
          <q-tabs
            v-model="tab"
            vertical
            class="text-dark"
        
          >
            <q-tab name="module1" class="q-my-md">
                <div style="text-align: left!important;">
                    <div class="text-blue-grey-13">MODULE-1</div>
                    <div class="text-h6">Programming Language Fundamentals</div>
                </div>
            </q-tab>
            <q-tab name="module2" class="q-my-md">
                <div style="text-align: left!important;">
                    <div class="text-blue-grey-13">MODULE-2</div>
                    <div class="text-h6">Data Structures and Algorithms</div>
                </div>
            </q-tab>
            <q-tab name="module3" class="q-my-md">
                <div style="text-align: left!important;">
                    <div class="text-blue-grey-13">MODULE-3</div>
                    <div class="text-h6">SQL</div>
                </div>
            </q-tab>
            <q-tab name="module4" class="q-my-md">
                <div style="text-align: left!important;">
                    <div class="text-blue-grey-13">MODULE-4</div>
                    <div class="text-h6">LLD and Project Specialisations</div>
                </div>
            </q-tab>
            <q-tab name="module5" class="q-my-md">
                <div style="text-align: left!important;">
                    <div class="text-blue-grey-13">MODULE-5</div>
                    <div class="text-h6">System Design Essentials</div>
                </div>
            </q-tab>
            <q-tab name="module6" class="q-my-md">
                <div style="text-align: left!important;">
                    <div class="text-blue-grey-13">MODULE-6</div>
                    <div class="text-h6">Electives</div>
                </div>
            </q-tab>
        </q-tabs>
        </template>
  
        <template v-slot:after>
          <q-tab-panels
            style="width: 500px;"
            v-model="tab"
            animated
            swipeable
            vertical
            transition-prev="jump-up"
            transition-next="jump-up"
          >
            <q-tab-panel name="module1">
              <div class="text-h3 q-mb-md">2 Months</div>
              <hr>
              <div>
                <div>
                    Introduction to Problem Solving
                </div>
                <div>
                    <ul>
                        <li>Introduction to Java</li>
                        <li>Input Output and Data Types</li>
                        <li>Operators</li>
                        <li>Conditions</li>
                        <li>Loops</li>
                        <li>Pattern Problems</li>
                        <li>Functions</li>
                        <li>1D and 2D Arrays</li>
                        <li>Strings</li>
                        <li>Memory Management</li>
                        <li>Basic OOP for Problem Solving</li>
                    </ul>
                </div>
              </div>
            </q-tab-panel>
  
            <q-tab-panel name="module2">
              <div class="text-h3 q-mb-md">4.5 Months</div>
              <hr>
              <div>
                <div>
                  Data Structures and Algorithms
                </div>
                <div>
                    <ul>
                        <li>Time and Space Complexity</li>
                        <li>Array Problem Solving Techniques</li>
                        <li>Bit Manipulation</li>
                        <li>Maths for Problem Solving</li>
                        <li>Recursion</li>
                        <li>Backtracking</li>
                        <li>Sorting</li>
                        <li>Searching(Binary Search)</li>
                        <li>Two Pointers</li>
                        <li>Hashing</li>
                        <li>Strings and Pattern Matching</li>
                    </ul>
                </div>
                <div>
                  Data Structures
                </div>
                <div>
                    <ul>
                        <li>Linked Lists</li>
                        <li>Stacks</li>
                        <li>Queues and Deques</li>
                        <li>Tree and BST</li>
                        <li>Tiers</li>
                        <li>Heaps</li>
                    </ul>
                </div>
                <div>
                  Advanced Problem Solving Techniques
                </div>
                <div>
                    <ul>
                        <li>Greedy</li>
                        <li>Dynamic Programming</li>
                        <li>Graphs</li>
                    </ul>
                </div>
              </div>
            </q-tab-panel>
  
            <q-tab-panel name="module3">
              <div class="text-h3 q-mb-md">0.5 Months</div>
              <hr>
              <div>
                <div>
                  SQL
                </div>
                <div>
                    <ul>
                        <li>Relational Model</li>
                        <li>CURD</li>
                        <li>Joins</li>
                        <li>Aggregation</li>
                        <li>Subqueries</li>
                        <li>Views</li>
                        <li>Transactions</li>
                        <li>Indexing</li>
                    </ul>
                </div>
              </div>
            </q-tab-panel>

            <q-tab-panel name="module4">
              <div class="text-h3 q-mb-md">3.5 Months</div>
              <p>*Only 1 Specialisation is allowed per learner. Recorded lectures for the other can be availed via Student Dashboard. At Least 1 Specialisation is mandatory for successful completion of the course.</p>
              <hr>
              <div>
                <div>
                  Fullstack Engineering
                </div>
                <div>
                    <ul>
                      <li>HTML, CSS, Javascript</li>
                      <li>Advanced HTML, CSS Case Studies</li>
                      <li>Advanced JS Concepts (OOP and Concurrency) and Popular Interview Questions</li>
                      <li>JS for Web Dev (DOM Manipulation, Event Handling)</li>
                      <li>Design Patterns</li>
                      <li>Git</li>
                      <li>React</li>
                      <li>Redux</li>
                      <li>How Internet Works (TCP, UDP, HTTP, Layering Architecture)</li>
                      <li>API Design</li>
                      <li>Deployment</li>
                      <li>Frontend LLD and Machine Coding Case Studies</li>
                      <li>Testing</li>
                      <li>MongoDB</li>
                      <li>NodeJS</li>
                      <li>ExpressJS</li>
                      <li>Backend Architecture</li>
                      <li>Capstone Projects</li>
                    </ul>
                </div>
                <div class="text-center">Or</div>
                <div>
                  Backend Engineering
                </div>
                <div>
                    <ul>
                      <li>OOP</li>
                      <li>Multithreading</li>
                      <li>Adv Lang Concepts and Popular Interview Questions</li>
                      <li>SOLID</li>
                      <li>Design Patterns</li>
                      <li>UML Diagrams</li>
                      <li>Schema Design</li>
                      <li>How Internet Works (TCP, UDP, HTTP, Layering Architecture)</li>
                      <li>API Design</li>
                      <li>MVC</li>
                      <li>Backend LLD and Machine Coding Case Studies</li>
                      <li>Unit Testing</li>
                      <li>ORM</li>
                      <li>Deployment</li>
                      <li>Git</li>
                      <li>Spring Boot</li>
                      <li>Project Interview Questions (Spring/Hibernate)</li>
                      <li>Capstone Projects (include advance things like implementing Payment API)</li>
                    </ul>
                </div>
              </div>
            </q-tab-panel>

            <q-tab-panel name="module5">
              <div class="text-h3 q-mb-md">1 Month</div>
              <hr>
              <div>
                <div>
                  <ul>
                    <li>Introduction to Scale and Scaling Techniques</li>
                    <li>Introduction to Caching Techniques</li>
                    <li>Introduction to SQL and NoSQL Databases</li>
                    <li>Introduction to Event Driven Architecture</li>
                    <li>Introduction to Microservice Architecture</li>
                  </ul>
                </div>
              </div>
            </q-tab-panel>

            <q-tab-panel name="module6">
              <div class="text-h3 q-mb-md">1-2 Months</div>
              <p>*A learner can do as many electives as they want, but only after completion of Core Curriculum.</p>
              <hr>
              <div>
                <div>
                  Advanced Software & System Design - 1.5 months
                </div>
                <div>
                    <ul>
                        <li>Consistent Hashing</li>
                        <li>Caching</li>
                        <li>CAP Theorem</li>
                        <li>Distributed Systems & Databases</li>
                        <li>SQL and NoSQL</li>
                        <li>Scalability</li>
                        <li>Zookeeper + Kafka</li>
                        <li>Location Based Services (S3, Quad Trees)</li>
                        <li>Strings</li>
                        <li>Microservices</li>
                        <li>Case Studies</li>
                    </ul>
                </div>
                <div class="text-center">And/Or</div>
                <div>
                  Data Engineering - 2 Months
                </div>
                <div>
                  <ul>
                    <li>Building efficient Data Processing Systems</li>
                    <li>Advanced SQL</li>
                    <li>Cloud Services - AWS, or GCP</li>
                    <li>Developing ETL pipelines</li>
                    <li>Map-Reduce Framework</li>
                    <li>Big Data</li>
                    <li>Data Warehousing & Modelling</li>
                    <li>OLAP, Dashboarding</li>
                    <li>Workflow Orchestration</li>
                    <li>Logging, and Monitoring</li>
                    <li>MapReduce, HiveQL, Presto</li>
                    <li>Projects</li>
                  </ul>
                </div>
                <div class="text-center">And/Or</div>
                <div>
                  DSA for Competitive Programming - 1 Months
                </div>
                <div>
                  <ul>
                    <li>Combinatorics and Probability</li>
                    <li>Matrix exponentiation</li>
                    <li>Advanced Trees: Segment Tree, k-D Tree</li>
                    <li>Disjoint Set Union</li>
                    <li>Advanced Dynamic Programming</li>
                    <li>Advanced Graphs: Bridges, Articulation point, Network Flow</li>
                  </ul>
                </div>
                <div class="text-center">And/Or</div>
                <div>
                  Product Management for Engineers - 1 Month
                </div>
                <div>
                  <ul>
                    <li>Introduction to Product Management</li>
                    <li>Product Thinking & Product Discovery</li>
                    <li>Product Roadmap & Prioritization</li>
                    <li>Mental Models for Product Managers</li>
                    <li>Product Analytics</li>
                    <li>Hands-on case study & Mixpanel session</li>
                    <li>Delivery & Project Management</li>
                    <li>Practical ways to apply PM lessons as an Engineer</li>
                  </ul>
                </div>
              </div>
            </q-tab-panel>
          </q-tab-panels>
        </template>
      </q-splitter>
    </div>
  </template>
  
  <script>
  import { ref } from 'vue'
  
  export default {
    name:'VerticalTab',
    setup () {
      return {
        tab: ref('module1'),
        splitterModel: ref(50)
      }
    }
  }
  </script>
  <style scoped>
  .flex-center, .justify-center {
    justify-content: initial;
    }
  </style>
  