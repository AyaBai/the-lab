<template>
  <div>
    <vue-final-modal v-model="showModal" classes="modal-container" content-class="modal-content">
      <button class="btn_red"></button>
     <!-- <span class="modal__title">Modal Content Here </span> -->
     <div class="container_modal">
       <div class="modal_left">
        <div class="modal_left_name">
          <div class="modal_left_head" >Вирусный гепатит А</div>
          <div class="modal_left_main">HBsAg</div>
          <div class="modal_left_footer">N: 0.001 – 4.000</div>
        </div>
        <div class="modal_input">
          <input type="text" class="modal_input_left" placeholder="_.___">
          <button class="modal_btn_right">Клавиатура</button>
        </div>

        <button class="modal_btn">
          Ложно положительный
        </button>

        <div class="modal_table_left">
          <table>
            <th class="table_left_head">тест система</th>
            <th class="table_right_head">остаток</th>
              <tr class="mt_left_row">
                <td  class="mt_left_column_1">IMDI 107</td>
                <td class="mt_left_column_2"> 96 / 96</td>
              </tr>   
               <tr class="mt_left_row active">
                <td  class="mt_left_column_1 active">MBU 19087-3</td>
                <td class="mt_left_column_2"> 1996 / 596</td>
              </tr>
              <tr class="mt_left_row">
                <td  class="mt_left_column_1">KF 39/4</td>
                <td class="mt_left_column_2">1235 / 45</td>
              </tr>    
          </table>
        </div>
        <div class="ml_btn_footer">
          <button class="btn_blue">Сохранить</button>
          <button class="btn_green">Расичтать</button>
        </div>



       </div>
       <!-- modal_right -->
       <div class="modal_right">
        
        <div class="modal_right_info">
          <div class="mr_data">
          <p class="mr_data_num">405</p>
          <p class="mr_data_name">Константин</p>
          <p class="mr_data_name">Константинопольский</p>
          </div>
          <div class="mr_data_iin">
            955 559 588 598
          </div>
        </div>

        <div class="modal_right_info2">
          <div class="mr_info2_data">
            <div class="mr_info2_cover">
              <div class="mr_info2_title">Пол</div>
              <div class="mr_info2_text">Женский</div>
            </div>
          </div>

          <div class="mr_info2_data">
            <div class="mr_info2_cover">
              <div pan class="mr_info2_title"> Возраст</div>
              <div pan class="mr_info2_text">26 лет</div>
            </div> 
          </div>

          <div class="mr_info2_data">
            <div class="mr_info2_cover">
              <div pan class="mr_info2_title">Беременность</div>
              <div class="mr_info2_text">2 неделя</div>
            </div>
          </div>

          <div class="mr_info2_data">
            <div class="mr_info2_cover">
              <div class="mr_info2_title">Цикл</div>
              <div class="mr_info2_text">3 день</div>
            </div>
          </div>
        </div>

        <div class="ordered_analysis">
          <div class="ordered_analysis_left">
            <div>1</div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
          </div>
          <div class="ordered_analysis_right">
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
            <div></div>
          </div>
        </div>

       </div><!-- modal_right end -->


     </div>

     <div class="modal__action">
        <button highlight @click="showConfirmModal = true">confirm</button>
        <button @click="showModal = false">cancel</button>
      </div>

    </vue-final-modal>
  </div>
  <div class="container_results">
    <div>Хламидиоз  (трахоматис)</div>
    <div  class="results">
      <div v-for="item in items" :key="item.number">
        <span class="number"> {{item.number}}</span><br>
        <span class="person_data_result">_.___</span><br>
        <span class="person_data">{{item.gender}}</span><br>
        <span class="person_data">{{item.age}}</span>
      </div>
    </div>
  
    <div>Хламидиоза (пневмония)  IgM</div>
    <div  class="results">
      <div v-for="item in items" :key="item.number">
        <span class="number"> {{item.number}}</span><br>
        <span class="person_data_result">_.___</span><br>
        <span class="person_data">{{item.gender}}</span><br>
        <span class="person_data">{{item.age}}</span>
      </div>
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
            gender:'мужской', 
            age:'26 лет'
          },
          {
            number:'05',
            result:'',  
            gender:'мужской', 
            age:'26 лет'
          },
          {
            number:'07',
            result:'',  
            gender:'мужской', 
            age:'26 лет'
          },
          {
            number:'09',
            result:'',  
            gender:'мужской', 
            age:'26 лет'
          },
          {
            number:'10',
            result:'',  
            gender:'мужской', 
            age:'26 лет'
          },
           {
            number:'12',
            result:'',  
            gender:'мужской', 
            age:'26 лет'
          },
           {
            number:'16',
            result:'',  
            gender:'мужской', 
            age:'26 лет'
          },
          {
            number:'22',
            result:'',  
            gender:'мужской', 
            age:'26 лет'
          },
          {
            number:'25',
            result:'',  
            gender:'мужской', 
            age:'26 лет'
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


/* Modal */

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
    border-radius: 16px;
    position: relative;
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

.container_results {
  width: 100%;
  margin-left: 24px;
  color: #3F3F46;
}

.container_modal {
  width: 749px;
  height: 564px;
  display: flex;
  justify-content: space-between;
  flex-direction: row;

}

.modal_left {
  width: 289px;
  height: 100%;
/*  outline: 1px solid lightblue;*/
  margin: 12px 12px 89px;

}



.modal_left_name {
  width: 289px;
  height: 180px;
/*  outline: 2px solid #0075FF;*/
  filter: drop-shadow(0px 4px 4px rgba(0, 0, 0, 0.25));
  background: radial-gradient(173.88% 150.92% at 110.9% 88.82%, rgba(5, 0, 255, 0.1) 20.27%, rgba(0, 255, 255, 0.1) 23.95%, rgba(72, 255, 200, 0.1) 25.7%, rgba(0, 113, 218, 0.070757) 30.65%, rgba(255, 255, 255, 0) 38.58%) /* warning: gradient uses a rotation that is not supported by CSS and may not behave as expected */, radial-gradient(124.57% 172.37% at 12.46% 17.54%, rgba(9, 152, 255, 0.69) 0%, rgba(0, 228, 215, 0.69) 26.61%, rgba(0, 205, 196, 0) 41.99%) /* warning: gradient uses a rotation that is not supported by CSS and may not behave as expected */, #0075FF;
  background-color: #0075FF;
  border-radius: 16px;
  position: relative;
  color: #fff;
  margin-bottom: 12px;
}

.modal_left_head {
  position: absolute;
  font-size: 14px;
  letter-spacing: 0.3px;
  color: #FAFAFA;
  left: 12px;
  top: 21px;

}

.modal_left_main {
  position: absolute;
  left: 12px;
  top: 43px;
  letter-spacing: 0.1px;
  font-size: 48px;
}

.modal_left_footer {
  position: absolute;
  left: 12px;
  bottom: 20px;
  letter-spacing: 0.3px;
  font-size: 16px;
}

.modal_input {
  width: 266px;
  height: 60px;
  display: flex;
/*  align-items: center;*/
  flex-direction: row;
  border: 1px solid #71717A;
  border-radius: 8px;
  outline: none;
  margin-left: 11px;
  margin-bottom: 12px;
  overflow: hidden;
}

.modal_input_left, .modal_btn_right {
  color: #71717A;
  height: inherit;
  border: 0;
  text-align: center;

}

.modal_input_left {
  width: 132px;
  font-size: 24px;
  font-weight: 500;
  letter-spacing: 0.1px;
/*  padding-left: 43px;*/
  outline: none;

}

.modal_btn_right {
  width: 134px;
/*  padding-left: 27px;*/
  outline: none;
  border-left: 1px solid #71717A;
  background-color: #fff;

}

.modal_btn {
  width: 266px;
  height: 48px;
  margin-left: 12px;
  background-color: #EA580C;
  color: #FFFFFF;
  border-radius: 8px;
  border: none;
  margin-bottom: 9px;
}

.modal_table_left {
  width: 100%;
  height: 94px;
/*  padding-left: 12px;*/
  margin-bottom: 89px;
  border-collapse: collapse;
/*  padding: 0;*/
/*  outline: 2px solid red;*/
}

.modal_table_left>table {
/*  border: 2px solid  green;*/
  color: #3F3F46;
  font-weight: 300;
  font-size: 14px;
  width: inherit;
  padding: 0;
}

.table_left_head,
.table_right_head {
  color: #A1A1AA;
  font-weight: 300;
  font-size: 14px;
  letter-spacing: 0.3px;
  padding-left: 12px;
}

.table_right_head {
  text-align: right;
  padding-right: 12px;
}

.mt_left_row {


}

.mt_left_column_1, .mt_left_column_2 {
/*  outline: 1px solid red;*/
  height: 24px;
  padding: 0;
}

.mt_left_column_1 {
  
  width: 157px;
  padding-left: 12px;
  
}

.mt_left_column_2 {
  text-align: right;
  width: 132px;
   padding-right: 12px;
}

.table_left_head {
  text-align: left;
}

.ml_btn_footer{
  display: flex;
  justify-content: space-between;

}

.btn_blue,
.btn_green {
  width: 127px;
  height: 36px;  
  border-radius: 34px;
  color: #FFFFFF;
  border: none;
}

.btn_blue {
  background: #0085FF;

}

.btn_green {
  background: #00CCB1;

}

.active {
  background-color: #0098EA;
  border: 2px solid #0098EA;
}


/*modal right*/



.modal_right {
  width: 424px;
  outline: 1px solid hotpink;
  height: 100%;
  margin: 12px 12px 24px;
  

}

.btn_red {
  background-color: #DC2626;
  background-image: url(../img/clear.svg);
  background-position: center;
  width: 19px;
  height: 19px;
  border-radius: 50%;
  border: none;
  position: absolute;
  top: 17px;
  right: 12px;
} 

.modal_right_info{
  display: flex;
  flex-direction: row;
  width: inherit;
/*  outline: 1px solid red;*/
  position: relative;
  margin-bottom: 30px;
}
.mr_data { 
  width: 310px;

}

.mr_data_num {
  font-weight: 500;
  font-size: 16px;
  color: #52525B;
  letter-spacing: 0.1px;
  margin-bottom: 4px;
  width: 100%;

}

.mr_data_name,
.mr_data_iin {
  color: #3F3F46;
  
}
 
.mr_data_name {
  font-weight: 400;
  font-size: 16px;
  letter-spacing: 0.1px;
  width: 320px;


}

.mr_data_iin {
  width: 110px;
  height: 18px;
  font-size: 14px;
  font-weight: 300;
  position: absolute;
  bottom: 0;
  right: 0;
}

.modal_right_info2 {
/*  outline: 2px solid green;*/
  height: 72px;
  width: 100%;
  display: flex;
  flex-direction: row;
  margin-bottom: 12px;
}

.mr_info2_data {
  height: inherit;
  width: 100px;
  margin-right: 8px;
  border: 1px solid #F4F4F5;
  border-radius: 16px;
  position: relative;
}

.mr_info2_cover {
  position: absolute;
  top: 14px;
  left: 11px;
}

.mr_info2_title {
  font-weight: 300;
  font-size: 12px;
  color: #71717A;
  letter-spacing: 0.4px;
  margin-bottom: 3px;


}
.mr_info2_text {
  font-weight: 400;
  font-size: 16px;
  color: #3F3F46;
  letter-spacing: 0.1px;
}

.ordered_analysis {
  width: 423px;
  height: 300px;
  background: #FAFAFA;
  border-radius: 16px;
  outline: 2px solid red;
  display: flex;
  flex-direction: row;
}

.ordered_analysis_left {
  width: 174px;
  height: 100%;
  outline: 2px solid hotpink;
  margin: 20px 0 31px 12px;
}

.ordered_analysis_right {
  width: 202px;
  height: 100%;
  outline: 2px solid blue;
}
</style>