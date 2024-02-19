<template>
    <div class="q-pa-md">
      <div class="q-gutter-y-md">
        <q-option-group
          v-model="panel"
          inline
          :options="[
            { label: 'Beginner', value: 'Beginner' },
            { label: 'Intermediate', value: 'Intermediate' },
            { label: 'Advanced', value: 'Advanced' }
          ]"
        />
  
        <q-tab-panels v-model="panel" animated class="shadow-2 rounded-borders">
          <q-tab-panel name="Beginner">
            <div class="text-h6 text-center">11.5 Months</div>
            <div class="q-pa-sm">
                <q-list bordered class="rounded-borders">
                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Programming Language Fundamentals</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                Data Structures and Algorithms
                            </q-item-section>     
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white">
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                Data Structures
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white">
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Advanced Problem Solving Techniques</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Programming Language Fundamentals</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Programming Language Fundamentals</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>
                </q-list>
            </div>
          </q-tab-panel>
  
          <q-tab-panel name="Intermediate">
            <div class="text-h6 text-center">11.5 Months</div>
            <div class="q-pa-sm">
                <q-list bordered class="rounded-borders">
                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Programming Language Fundamentals</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                Data Structures and Algorithms
                            </q-item-section>     
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white">
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                Data Structures
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white">
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Advanced Problem Solving Techniques</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Programming Language Fundamentals</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Programming Language Fundamentals</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>
                </q-list>
            </div>
          </q-tab-panel>
  
          <q-tab-panel name="Advanced">
            <div class="text-h6 text-center">9.5 Months</div>
            <div class="q-pa-sm">
                <q-list bordered class="rounded-borders">
                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Programming Language Fundamentals</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                Data Structures and Algorithms
                            </q-item-section>     
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white">
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                Data Structures
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white">
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Advanced Problem Solving Techniques</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Programming Language Fundamentals</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>

                    <q-separator />

                    <q-expansion-item>
                        <template v-slot:header>
                            <q-item-section>
                                <div>Programming Language Fundamentals</div>
                            </q-item-section>
                        </template>

                        <q-card>
                            <q-card-section class="bg-indigo-5 text-white"> 
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
                            </q-card-section>
                        </q-card>
                    </q-expansion-item>
                </q-list>
            </div>
          </q-tab-panel>
        </q-tab-panels>
      </div>
    </div>
  </template>
  
  <script>
  import { ref } from 'vue'
 
  export default { 
    name:'TabAccordian',
    setup () {
      return {
        panel: ref('Beginner')
      }
    }
  }
  </script>
  