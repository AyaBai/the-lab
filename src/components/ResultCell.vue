<template>
  <div>
    <vue-final-modal v-model="showModal" classes="modal-container" content-class="modal-content">
     <span class="modal__title">Modal Content Here </span>
     <div class="modal__action">
        <button highlight @click="showConfirmModal = true">confirm</button>
        <button @click="showModal = false">cancel</button>
      </div>

    </vue-final-modal>
  </div>
  
  <div>Хламидиоз  (трахоматис)</div>
  <div  class="results">
    
    <div v-for="item in items" :key="item.number">
      <span class="number"> {{item.number}}</span><br>
      <span class="person_data_result">_.___</span><br>
      <span class="person_data">{{item.gender}}</span><br>
      <span class="person_data">{{item.age}}</span>
    </div>
  </div>

</template>


<script>
  import { VueFinalModal } from 'vue-final-modal'

  export default {
    components: {
      VueFinalModal
    },

    data() {
      return {
        showModal: true,
        items: [
          {
            number:'01',
            result:'',
            gender:'мужской', 
            age:'26 лет'
          },
          {
            number:'02',
            result:'',  
            gender:'женский', 
            age:'20 лет'
          },
          {
            number:'05',
            result:'',  
            gender:'мужской', 
            age:'24 лет'
          },
          {
            number:'07',
            result:'',  
            gender:'мужской', 
            age:'24 лет'
          },
          {
            number:'09',
            result:'',  
            gender:'мужской', 
            age:'24 лет'
          },
          {
            number:'10',
            result:'',  
            gender:'мужской', 
            age:'24 лет'
          },
        ]
        
      }
    }
  }
  
</script>

<style scoped>
  .results {
    
/*    outline: 2px solid blue;*/
    height: 276px;
    width: 100%;
    flex-direction: row;
    overflow: hidden;
    flex-wrap: wrap;
    margin-left: 70px;
    padding: 5px;

  }

  :deep .modal-container {
  display: flex;
  justify-content: center;
  align-items: center;
  }

  :deep .modal-content {
    display: flex;
    flex-direction: column;
    margin: 0 1rem;
    padding: 1rem;
    border: 1px solid #e2e8f0;
    border-radius: 0.25rem;
    background: #fff;
  }
  .modal__title {
    font-size: 1.5rem;
    font-weight: 700;
  }
  .modal__action {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-shrink: 0;
  padding: 1rem 0 0;
}

</style>