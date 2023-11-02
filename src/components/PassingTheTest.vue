<template>
  <div v-if="!quizCompleted">
    <div class="container">
      <header class="h-main-home">
        <div class="header-home">
          <div class="h-main-title">Testing</div>
        </div>
      </header>

      <div class="main-header-passing">
        <div class="header-passing">

          <div class="header-passing-timer">
            <div class="passing-timer">
              <svg
                  viewBox="0 0 27 30"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                  height="22px"
                  width="17px"
                  class="icon-watch-time"
              >
                <path d="M14.3101 30C13.7635 30 13.2162 30 12.6696 30C12.5742 29.9824 12.4803 29.956 12.3842 29.9486C11.3776 29.8753 10.3842 29.7087 9.43481 29.3712C4.09442 27.4725 0.936706 23.7344 0.129668 18.1123C-0.289258 15.1923 0.320419 12.4271 1.76282 9.85045C1.85673 9.68318 1.94844 9.5159 2.05482 9.32442C1.7863 9.06616 1.52657 8.82992 1.28153 8.57827C0.356369 7.63037 0.349035 6.37506 1.26612 5.41762C1.63736 5.02951 2.01887 4.65166 2.40331 4.27602C3.36809 3.33252 4.64468 3.33619 5.60725 4.28482C5.8567 4.5306 6.09294 4.79106 6.34093 5.05005C8.27928 3.84463 10.3585 3.18725 12.594 3.02658C12.594 2.59004 12.594 2.1858 12.594 1.75733C12.1487 1.75733 11.7202 1.7698 11.2932 1.75366C10.809 1.73532 10.4458 1.34795 10.4458 0.87913C10.4465 0.411048 10.8104 0.0119313 11.2947 0.00826295C12.7591 -0.00347579 14.2242 -0.00200844 15.6894 0.00826295C16.0643 0.0111976 16.3357 0.218085 16.4744 0.56878C16.7004 1.13958 16.291 1.73605 15.6571 1.75586C15.2323 1.76907 14.8068 1.75807 14.3922 1.75807C14.3922 2.20854 14.3922 2.61353 14.3922 2.98623C15.1677 3.11976 15.9256 3.21 16.6622 3.38608C18.9586 3.93413 20.9696 5.02657 22.6901 6.64798C25.3525 9.15787 26.7839 12.2525 26.9475 15.8944C27.109 19.4806 25.9989 22.6655 23.6336 25.3771C21.5741 27.7381 18.9916 29.2135 15.9007 29.7748C15.3739 29.8709 14.8405 29.9259 14.3101 30ZM14.3688 7.40366C14.3688 7.50197 14.3688 7.59735 14.3688 7.69273C14.3688 8.20043 14.3746 8.70813 14.3658 9.21583C14.3585 9.65897 14.0782 10.0031 13.6798 10.0845C13.1164 10.1997 12.6256 9.80937 12.6138 9.21876C12.6021 8.61568 12.6109 8.01188 12.6109 7.4066C8.10614 7.78077 4.68649 11.6157 4.42678 15.623C4.53389 15.623 4.63881 15.6222 4.74446 15.623C5.26169 15.6259 5.77967 15.6127 6.29617 15.6369C6.75398 15.6582 7.09294 16.0368 7.09954 16.4858C7.10615 16.9216 6.79287 17.3082 6.34973 17.3544C6.00197 17.3904 5.64834 17.3764 5.29691 17.3809C5.00711 17.3845 4.71731 17.3816 4.42531 17.3816C4.72098 21.6237 8.38493 25.2964 12.6094 25.5804C12.6094 25.4733 12.6094 25.3669 12.6094 25.2612C12.6101 24.7535 12.5984 24.2458 12.6145 23.7388C12.6307 23.248 13.0085 22.8966 13.4861 22.8959C13.9638 22.8951 14.3335 23.2465 14.3636 23.7359C14.3724 23.8819 14.3666 24.0286 14.3666 24.1754C14.3666 24.6493 14.3666 25.1233 14.3666 25.6002C18.9711 25.1695 22.2682 21.3427 22.5529 17.3831C22.4377 17.3831 22.3232 17.3845 22.2088 17.3831C21.682 17.3765 21.1537 17.3919 20.6284 17.3552C20.2168 17.3266 19.9175 16.9825 19.8801 16.5782C19.8434 16.1908 20.076 15.8079 20.4509 15.6853C20.6042 15.6354 20.7766 15.6296 20.941 15.6274C21.4766 15.6208 22.0121 15.6252 22.5484 15.6252C22.3107 11.7169 18.974 7.80351 14.3688 7.40366Z" fill="#F7C844"/>
                <path d="M14.4222 15.9942C14.847 15.9942 15.2263 15.9906 15.6057 15.995C16.1515 16.0016 16.5382 16.3713 16.5352 16.8754C16.5323 17.364 16.15 17.7411 15.624 17.7484C14.9409 17.758 14.2572 17.7587 13.5741 17.7484C13.0195 17.7396 12.6688 17.3772 12.6666 16.8167C12.6614 15.3721 12.6614 13.9275 12.6666 12.4829C12.668 11.9502 13.0305 11.5687 13.5228 11.5563C14.0136 11.5438 14.4149 11.9407 14.4193 12.4778C14.4288 13.532 14.4222 14.5863 14.423 15.6399C14.4222 15.7455 14.4222 15.8512 14.4222 15.9942Z" fill="#F7C844"/>
              </svg>
            </div>
            <div class="passing-text-timer">
              {{fillTime(min)}}:{{fillTime(sec)}}
            </div>
          </div>

          <div class="header-passing-title">
            <div class="passing-text-title">
              Question {{ currentQuestion+1 }} of {{ questions.length }}
            </div>
          </div>

          <div class="header-passing-rate">
            <div class="header-rate-correct">
              <div class="passing-rate-correct">
                <svg
                    width="30"
                    height="24"
                    class="icon-checkmark"
                    viewBox="0 0 30 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M0 12.2296C0.146997 11.5277 0.56781 11.0046 1.08374 10.5377C1.30063 10.3417 1.49807 10.1241 1.70704 9.9187C2.69206 8.95097 4.07124 8.94592 5.05194 9.92085C6.77555 11.6351 8.49124 13.3573 10.2098 15.0758C10.2646 15.1306 10.3222 15.1832 10.4 15.2581C10.4851 15.1774 10.5687 15.1025 10.6479 15.0232C15.377 10.2948 20.1054 5.56571 24.8346 0.83731C25.9486 -0.276696 27.2773 -0.278857 28.3884 0.829385C28.6579 1.09816 28.9274 1.36693 29.1962 1.63714C30.2648 2.71152 30.2691 4.06187 29.202 5.1312C27.5814 6.75538 25.9579 8.37595 24.3359 9.99868C20.1112 14.2234 15.8865 18.4481 11.6618 22.6728C10.8209 23.5138 9.98643 23.5145 9.14624 22.6743C6.46787 19.9959 3.79382 17.3125 1.10752 14.6428C0.608884 14.1477 0.157085 13.6405 0 12.9321C0 12.6979 0 12.4638 0 12.2296Z" fill="#74CA8F"/>
                </svg>
              </div>
              <div class="passing-text-correct">Correct: {{ getCorrect }}</div>
            </div>
            <div class="header-rate-wrong">
              <div class="passing-rate-wrong">
                <svg
                    width="30"
                    height="30"
                    class="icon-cross"
                    viewBox="0 0 30 30" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <rect width="6.4484" height="35.978" rx="2" transform="matrix(-0.707107 -0.707107 -0.707107 0.707107 30 4.55975)" fill="#DF506E"/>
                  <rect y="4.55975" width="6.4484" height="35.978" rx="2" transform="rotate(-45 0 4.55975)" fill="#DF506E"/>
                </svg>
              </div>
              <div class="passing-text-wrong">Wrong: {{ getWrong }}</div>
            </div>
          </div>
        </div>
      </div>

      <section class="main-question-block">
        <div class="question-block">
          <div class="question-content">
            <p class="question-text">
              {{ getCurrentQuestion.question }}
            </p>
            <div v-if="getCurrentQuestion.mediaUrl !== ''">
              <YouTube
                  :src="getCurrentQuestion.mediaUrl"
                  @ready="onReady"
                  ref="youtube" />
            </div>
            <div v-if="getCurrentQuestion.imageUrl !== ''">
              <img :src=getCurrentQuestion.imageUrl>
            </div>
          </div>
        </div>
      </section>

      <main class="main-answer-block">
        <div class="answer-block">
          <section class="quiz">
            <div class="options">
              <label
                  v-for="(option, index) in getCurrentQuestion.options"
                  :for="'option' + index" :key="index"
                  :class="`option
                ${
                   getCurrentQuestion.selected == index && this.isActive == false
                   ? 'selected'
                   : ''
                }
                ${
                  getCurrentQuestion.selected != null &&
                  index != this.getCurrentQuestion.selected
                    ? 'disabled'
                    : ''
                }
                ${
                  this.isActive == true
                    ? index == getCurrentQuestion.answer && this.isActive == true
                      ? 'correct'
                      : 'wrong'
                    : ''
                }`
                ">
                <input
                    type="radio"
                    :id="'option' + index"
                    :name="getCurrentQuestion.index"
                    :value="index"
                    v-model="getCurrentQuestion.selected"
                    @change="SetAnswer"
                />
                <span>{{ option }}</span>
              </label>
            </div>

            <div class="answer-btn">
              <button
                  class="answer-btn-submit"
                  @click="NextQuestion"
                  :disabled="!getCurrentQuestion.selected">
                {{
                  currentQuestion == questions.length - 1
                      ? 'Finish'
                      : getCurrentQuestion.selected == null
                      ? 'Select the variant'
                      : 'Next question'
                }}
              </button>
            </div>

          </section>
        </div>
      </main>
    </div>
  </div>

  <div v-else>
    <ResultThePassing
        :questions="questions.length"
        :getCorrect="getCorrect"
        :getWrong="getWrong"
        :getTimer="intervalList"
    />
  </div>
</template>

<script>
import ResultThePassing from './ResultTheTest';
import YouTube from "vue3-youtube";
// import VideoPlayer from "@/components/VideoPlayer";

export default {
  name: 'PassingTheTest',
  data: () => ({
    questions: [
      {
        question: 'What is Vue?',
        answer: 0,
        mediaUrl: 'https://www.youtube.com/watch?v=53kB0GKAd2k',
        imageUrl: '',
        options: [
          'test_1 (right)',
          'test_2',
          'test_3',
          'test_4'
        ],
        selected: null
      },
      {
        question: 'What is Vue?',
        answer: 0,
        mediaUrl: 'https://www.youtube.com/watch?v=4dW2KzlYaR4',
        imageUrl: '',
        options: [
          'A framework (right)',
          'A library',
          'A type of hat',
          'A something for test'
        ],
        selected: null
      },
      {
        question: 'What is Vuex used for?',
        answer: 2,
        mediaUrl: '',
        imageUrl: 'http://thumb7.shutterstock.com/display_pic_with_logo/2892448/342092249/stock-vector-cool-comic-book-bubble-text-pop-art-retro-style-342092249.jpg',
        options: [
          'Eating a delicious snack',
          'Viewing things',
          'State management (right)',
          'A something for test'
        ],
        selected: null
      },
      {
        question: 'What is Vue Router?',
        answer: 1,
        mediaUrl: '',
        imageUrl: 'https://images.ctfassets.net/hrltx12pl8hq/7yQR5uJhwEkRfjwMFJ7bUK/dc52a0913e8ff8b5c276177890eb0129/offset_comp_772626-opt.jpg?fit=fill&w=800&h=300',
        options: [
          'An ice cream maker',
          'A routing library for Vue (right)',
          'Burger sauce',
          'A something for test'
        ],
        selected: null
      },
      {
        question: 'Where is my head?',
        answer: 1,
        mediaUrl: '',
        imageUrl: '',
        options: [
          'A something for test-1',
          'A something for test-2 (right)',
          'A something for test-3',
          'A something for test-4',
        ],
        selected: null
      }
    ],
    quizCompleted: false,
    currentQuestion: 0,
    sec: 0,
    min: 0,
    hour: 0,
    timer: null,
    intervalList: [],
    isActive: false
  }),
  computed: {
    score() {
        let value = 0
        this.questions.map(q => {
          if (q.selected != null && q.answer == q.selected) {
            console.log('correct');
            value++
          }
        })
        return value
    },
    getCorrect() {
        let value = 0
        this.questions.map(q => {
          if (q.selected != null && q.answer == q.selected) {
            console.log('correct');
            value++
          }
        })
        return value
    },
    getWrong() {
        let value = 0
        this.questions.map(q => {
          if (q.selected != null && q.selected != q.answer) {
            console.log('wrong');
            value++
          }
        })
        return value
    },
    getCurrentQuestion() {
      let question = this.questions[this.currentQuestion]
      return question
    },
  },
  components: {
    ResultThePassing,
    YouTube
    // VideoPlayer
  },
  async mounted() {
    if(this.timer === null){
      this.playing()
      this.timer = setInterval(()=> this.playing(), 1000)
    }
    else{
      clearInterval(this.timer);
      this.timer = null;
      this.pause();
    }
  },
  methods: {
    onReady() {
      this.$refs.youtube.playVideo()
    },
    SetAnswer(e) {
      this.questions[this.currentQuestion].selected = e.target.value
      e.target.value = null
    },
    NextQuestion() {
      if (this.isActive === false) {
        this.isActive = true
      }

      if (this.currentQuestion < this.questions.length-1) {
        let interval = setTimeout(() => {
          // this.recieveAnswer()
          this.currentQuestion++
          this.isActive = false
        }, 1000);
        return interval
      }

      this.quizCompleted = true
      if(this.quizCompleted === true) {
        this.intervalList.push(`${this.fillTime(this.min)}:${this.fillTime(this.sec)}`)
      }
    },
    fillTime(number){
      return number.toString().padStart(2,0)
    },
    playing() {
      this.sec++
      if(this.sec >= 59){
        this.sec = 0;
        this.min++;
      }
      if(this.min >= 59){
        this.min = 0;
        this.hour++;
      }
    },
    pause(){
      this.intervalList.push(`${this.fillTime(this.min)}:${this.fillTime(this.sec)}`)
      console.log(this.intervalList)
    },
    clear(){
      if(this.timer !== null){
        clearInterval(this.timer)
        this.timer = null
      }
      this.sec = 0;
      this.min = 0;
      this.hour = 0;
      this.clearIntervalList();
    },
    clearIntervalList(){
      this.intervalList = []
      console.log(this.intervalList)
    }
  }
}

</script>

<style>
body {
  background-color: #74CA8F;
}
.container {
  width: 1200px;
  margin-left: auto;
  margin-right: auto;
  padding: 100px;
}
p {
  margin: 0;
  padding: 0;
}
button {
  border: none;
  background-color: transparent;
}
h2 {
  font-size: 2rem;
  margin-bottom: 2rem;
  text-align: center;
}
/*ICONS*/
.passing-timer {
  width: 40px;
  height: 40px;
  background: #FEF8E0;
  border-radius: 6px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.icon-watch-time {
  fill: #F7C844;
  width: 19px;
  height: 22px;
}
.passing-rate-correct {
  width: 40px;
  height: 40px;
  background: #ECFEF4;
  border-radius: 6px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.icon-checkmark {
  fill: #74CA8F;
  width: 22px;
  height: 17px;
}
.passing-rate-wrong {
  width: 40px;
  height: 40px;
  background: #FDF5F8;
  border-radius: 6px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.icon-cross {
  fill: #DF506E;
  width: 22px;
  height: 17px;
}
/*Header Passing*/
.main-header-passing {
  background-color: white;
  border-radius: 0.625rem;
  height: 100px;
  width: 100%;
}
.header-passing {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 30px 40px;
}
.header-passing-timer {
  display: flex;
  justify-content: center;
  align-items: center;
}
.header-passing-title {
  display: flex;
  justify-content: center;
  align-items: center;
}
.h-main-title {
  color: #FFF;
  text-align: left;
  font-family: Public Sans, sans-serif;
  font-size: 26px;
  font-style: normal;
  font-weight: 700;
  line-height: 30px; /* 115.385% */
  text-transform: capitalize;
  margin-bottom: 30px;
}
.header-passing-rate {
  display: flex;
  justify-content: center;
  align-items: center;
}
.header-rate-correct {
  display: flex;
  justify-content: center;
  align-items: center;
}
.header-rate-wrong {
  display: flex;
  justify-content: center;
  align-items: center;
}
.passing-text-timer {
  font-family: Inter,Helvetica,sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 21px;
  text-align: center;
  color: #B5B5C2;
  margin: 0 0 0 10px;
}
.passing-text-title {
  font-family: Inter,Helvetica,sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 27px;
  text-align: center;
  color: #449DF0;
  margin: 0 0 0 160px;
}
.passing-text-correct {
  font-family: Inter,Helvetica,sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 21px;
  color: #B5B5C2;
  margin: 0 10px 0 10px;
}
.passing-text-wrong {
  font-family: Inter,Helvetica,sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 21px;
  color: #B5B5C2;
  margin: 0 0 0 10px;
}
/*Questions Passing*/
.main-question-block {
  background-color: white;
  border-radius: 0.625rem;
  width: 100%;
  margin: 20px 0;
}
.question-block {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 30px 40px;
}
.question-content {

}
.question-text {
  font-family: Inter,Helvetica,sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 21px;
  text-transform: capitalize;
  color: #191C30;
}
/*Answers Passing*/
.main-answer-block {
  background-color: white;
  border-radius: 0.625rem;
  width: 100%;
}
.answer-block {
  padding: 30px 40px;
}
.answer-content {
  display: grid;
  grid-template-columns: 2fr 2fr;
  gap: 10px;
}
.answer-cart {
  width: 585px;
  height: 66px;
  background: #FFFFFF;
  border: 1px dashed #E4E6EE;
  border-radius: 8px;
  display: flex;
  align-items: center;
  padding: 15px;
}
.answer-cart:hover {
  width: 585px;
  height: 66px;
  background: #F3FAFE;
  border: 1px dashed #449DF0;
  border-radius: 8px;

}
.event-answer-cart {
  padding: 0 15px 0 0;
}
.text-answer-cart {
  font-family: Inter,Helvetica,sans-serif;
  font-style: normal;
  font-weight: 600;
  font-size: 12px;
  line-height: 18px;
  text-transform: capitalize;

  color: #191C30;
}
.answer-btn {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 30px 0;
}
.answer-btn-submit {
  font-family: Inter,Helvetica,sans-serif;
  width: 186px;
  height: 42px;
  background: #449DF0;
  border-radius: 6px;
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  line-height: 21px;
  text-align: center;
  color: #FFFFFF;
}
/*QUIZ*/
.quiz {
  color: black;
  width: 100%;
}
.quiz-info {
}
.quiz-info .question {
  color: #8F8F8F;
  font-size: 1.25rem;
}
.quiz-info.score {
  color: #FFF;
  font-size: 1.25rem;
}
.options {
  display: grid;
  grid-template-columns: 2fr 2fr;
  gap: 10px;
}
.option {
  height: 66px;
  background: #FFFFFF;
  border: 1px dashed #E4E6EE;
  color: black;
  border-radius: 8px;
  display: flex;
  align-items: center;
  padding: 15px;

  transition: all .1s;
}
.option:hover {
  height: 66px;
  background: #F3FAFE;
  border: 1px dashed #449DF0;
  border-radius: 8px;
  cursor: pointer;
}
.option.selected {
  background: #FEF8E0;
  color: #F7C844;
  border: 1px solid #F7C844;
}
.option.correct {
  background-color: #ECFEF4;
  color: #74CA8F;
  border: 1px solid #74CA8F;
}
.option.wrong {
  background-color: #FDF5F8;
  color: #DF506E;
  border: 1px solid #DF506E;
}
.option:last-of-type {

}
.option.disabled {
  opacity: 0.5;
}
.option input {
  display: none;
}
button:disabled {
  opacity: 0.5;
}
@media (max-width: 750px) {
  .header-passing-rate {
    display: block;
  }
  .header-rate-correct {
    display: flex;
    justify-content: left;
    align-items: center;
  }
  .header-rate-wrong {
    display: flex;
    justify-content: left;
    align-items: center;
  }
  .passing-text-title {
    margin: 0 0 0 30px;
  }
  .passing-text-correct {
    font-family: Inter,Helvetica,sans-serif;
    font-style: normal;
    font-weight: 600;
    font-size: 14px;
    line-height: 21px;
    color: #B5B5C2;
    margin: 0 0 0 10px;
  }
  .passing-text-wrong {
    font-family: Inter,Helvetica,sans-serif;
    font-style: normal;
    font-weight: 600;
    font-size: 14px;
    line-height: 21px;
    color: #B5B5C2;
    margin: 0 0 0 10px;
  }
  .question-block {
    display: flex;
    justify-content: center;
  }
  .question-text {
    font-size: 18px;
  }
  .options {
    display: grid;
    grid-template-columns: 1fr;
  }
  .option {
    font-size: 16px;
  }
  .main-answer-block {
    height: 100%;
  }
}
</style>