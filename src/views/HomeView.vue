<script setup>
  import { ref,reactive} from 'vue'

  const quizzData = ref([
    {
      question: 'Which language runs in a web browser?',
      a: 'Java',
      b: 'C',
      c: 'Python',
      d: 'Javascript',
      correct: 'd'
    },
    {
      question: 'What does CSS stand for?',
      a: 'Central Style Sheet',
      b: 'Cascading Style Sheet',
      c: 'Cascading Simple Sheets',
      d: 'Core SUVs Sailboats',
      correct: 'b'
    },
    {
      question: 'What does HTML stand for?',
      a: 'HyperText Markup Language',
      b: 'HyperText Markdown Language',
      c: 'HyperText Machine Language',
      d: 'Helicopters Terminals Motorboats Lamborghinis',
      correct: 'a'
    },
    {
      question: 'What year was javascript invented?',
      a: '1996',
      b: '1995',
      c: '1994',
      d: 'none of the above',
      correct: 'b'
    },  
  ])
</script>

<template>
  <section>
    <div class="quiz-container">
      <div class="quiz-header">
        <h2 id="question">
          Question Text
        </h2>
      </div>
      <div>
        <ul>
          <li>
            <input type="radio" name="answer" id="" class="answer">
            <label for="">answer</label>
          </li>

          <li>
            <input type="radio" name="answer" id="" class="answer">
            <label for="">answer</label>
          </li>

          <li>
            <input type="radio" name="answer" id="" class="answer">
            <label for="">answer</label>
          </li>

          <li>
            <input type="radio" name="answer" id="" class="answer">
            <label for="">answer</label>
          </li>
        </ul>
      </div>


      <button>Submit</button>
    </div>
  </section>
</template>

<style scoped>
  *{
    box-sizing: border-box;
  }
  section{
    background-color: #b8c6db;
    background-image: linear-gradient(315deg, #b8c6db, #f5f2f7 100%);
    font-family: sans-serif;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
    margin: 0;
  }
  .quiz-container{
    background-color: #fff;
    border-radius: 10px;
    box-shadow: 0 0 10px 2px rgba(100,100,100,0.1);
    width: 600px;
    overflow: hidden;
    padding: 4rem;
  }
  /* .quiz-header{
    padding: 4rem;
  } */
  h2{
    padding: 1rem;
    text-align: center;
    margin: 0;
  }
  ul{
    list-style-type: none;
    padding: 0;
  }
  ul li{
    font-size: 1.2rem;
    margin: 1 rem 0;
  }
  ul li label{
    cursor: pointer;
  }
  button{
    background-color: #03cae4;
    border: none;
    border-radius: 5px;
    width: 150px;
    height: 30px;
    color: #fff;
    display: block;
    cursor: pointer;
    font-size: 1.1rem;
  }
</style>
