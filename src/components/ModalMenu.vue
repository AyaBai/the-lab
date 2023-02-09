<link rel="stylesheet" href="https://meyerweb.com/eric/tools/css/reset/reset.css">
<link rel="stylesheet" href="./fonts/stylesheet.css">
<template>
  <div class="test"><button @click="showModalMenu(item)">PopUp</button></div>

	<div>
    <vue-final-modal v-model="showModal" classes="modal-container" content-class="modal-content">
      <button class="btn_red"  @click="closeModal()"></button>
     
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
          <div>
            <div class="table_left_head">тест система</div>
            <div class="mt_left_row">
              <div class="mt_left_column_1"> IMDI 107</div>
              <div class="mt_left_column_1 active"> MBU 19087-3</div>
              <div class="mt_left_column_1">KF 39/4</div>
            </div>
          </div>

          <div class="mt_left_row">
            <div class="table_right_head">остаток</div>
            <div class="mt_left_row">
              <div class="mt_left_column_2"> 96 / 96</div>
              <div class="mt_left_column_2 active"> 1996 / 596</div>
              <div class="mt_left_column_2">1235 / 45</div>
            </div>
          </div>
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
            <p class="mr_data_num">{{cellNumber}}</p>
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
              <div class="mr_info2_text">{{cellGender}}</div>
            </div>
          </div>

          <div class="mr_info2_data">
            <div class="mr_info2_cover">
              <div pan class="mr_info2_title"> Возраст</div>
              <div pan class="mr_info2_text">{{cellAge}}</div>
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
            <div class="analysis_left_title">Заказанные анализы</div>
            <div class="analysis_left_body">Хламидиоза (трахоматис)</div>
            <div class="analysis_left_body">Микоплазма (пневмония)</div>
            <div class="analysis_left_body">Уреаплазмоза</div>
            <div class="analysis_left_body">Токсоплазмоза</div>
            <div class="analysis_left_body">Сифилиса</div>
            <div class="analysis_left_body">Зостер Варицелла</div>
            <div class="analysis_left_body">Кандидоза</div>
            <div class="analysis_left_body">Вирусный гепатит С</div>
            <div class="analysis_left_body">Кортизол</div>
            
          </div>
          <div class="ordered_analysis_right">
            <div class="analysis_right_title"><a href="#">История заказов</a></div>
            <div class="analysis_right_body">IgG IgM  IgA  авид  вЦик  Аффи.  sIgE</div>
            <div class="analysis_right_body">IgG</div>
            <div class="analysis_right_body">IgG  IgM  IgA</div>
            <div class="analysis_right_body">IgG  IgM  IgA  авид  вЦик  Аффи.  sIgE</div>
            <div class="analysis_right_body">IgG  IgM</div>
            <div class="analysis_right_body">IgG  IgM  IgA  авид  вЦик  Аффи.  sIgE</div>
            <div class="analysis_right_body">sIgE</div>
            <div class="analysis_right_body">АТ</div>
            <div class="analysis_right_body">--</div>
            
          </div>
        </div>

        <div class="btn_analysis">
            <button class="btn_analysis_left">
              <div class="btn_arrow_left"> 449</div>
            </button>
            <button class="btn_analysis_right">
              <div class="btn_arrow_right"> 450</div>
            </button>
          </div>

       </div><!-- modal_right end -->


     </div>

     <!-- <div class="modal__action">
        <button highlight @click="showConfirmModal = true">confirm</button>
        <button @click="showModal = false">cancel</button>
      </div> -->

    </vue-final-modal>
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
        showModal: false,
        cellNumber:'',
        cellAge:'',
        cellGendre:'',
      }
    },

    props: {
      items: {
        type: Array,
        required: true
      }
    },

    methods: {
      showModalMenu(item) {
        this.showModal = true
        this.cellNumber = item.number
        this.cellAge = item.age
        this.cellGender = item.gender
       
      },
      closeModal () {
        this.showModal = false
      },
      cellPopUp() {
        this.$emit('popUp', this.cellNumber)
      }
    }
  }
	

</script>

<style scoped>
  .test {
    outline: 2px solid red;
    width: 100px;
    height: 100px;
  }

  .test > button {
    width: 50px;
    height: 50px;
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
  color: #FAFAFA;
  left: 12px;
  top: 21px;

}

.modal_left_main {
  position: absolute;
  left: 12px;
  top: 43px;
  font-size: 48px;
}

.modal_left_footer {
  position: absolute;
  left: 12px;
  bottom: 20px;
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
/*  height: 94px;*/
/*  padding-left: 12px;*/
  margin-bottom: 89px;
  border-collapse: collapse;
  display: flex;
  flex-direction: row;
/*  padding: 0;*/
/*  outline: 2px solid red;*/
}

.modal_table_left>div {
/*  border: 2px solid  green;*/
  color: #3F3F46;
  font-weight: 300;
  font-size: 14px;
  width: inherit;
  padding: 0;
}

.table_left_head,
.table_right_head {
/*  height: 20px;*/
  color: #A1A1AA;
  font-weight: 300;
  font-size: 14px;
  padding-left: 12px;
  margin-bottom: 2px;
}

.table_right_head {
  text-align: right;
  padding-right: 12px;
}

.mt_left_row {


}

.mt_left_column_1, .mt_left_column_2 {
/*  outline: 1px solid red;*/
  padding: 3px;
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
/*  height: 36px;  */
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
  color: #FAFAFA;
}


/*modal right*/



.modal_right {
  width: 424px;
/*  outline: 1px solid hotpink;*/
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
  margin-bottom: 3px;


}
.mr_info2_text {
  font-weight: 400;
  font-size: 16px;
  color: #3F3F46;
}

.ordered_analysis {
  width: 423px;
  height: 300px;
  background: #FAFAFA;
  border-radius: 16px;
/*  outline: 2px solid red;*/
  display: flex;
  flex-direction: row;
  margin-bottom: 32px;
}

.ordered_analysis_left {
  width: 174px;
/*  height: 100%;*/
/*  outline: 2px solid hotpink;*/
  margin: 20px 0 31px 12px;
}

.ordered_analysis_right {
/*  width: 202px;*/
/*  height: 100%;*/
/*  outline: 2px solid blue;*/
  margin: 20px 3px 31px 24px;
}

.analysis_left_title {
  color: #3F3F46;
  font-weight: 400;
  font-size: 16px;
  margin-bottom: 18px;
}

.analysis_right_title {
  color: #0087D2;
  font-weight: 300;
  font-size: 14px;  
  text-align: right;
  margin-bottom: 20px;
}

.analysis_right_title>a {
  color: #0087D2;
  text-decoration: none; 
}

a:hover {
  color: #0087D2; 
  text-decoration: auto;
}

.analysis_left_body {
  color: #71717A;
  font-size: 14px;
  margin-bottom: 5px;
} 

.analysis_right_body {
  color: #18181B;
  text-align: right;
  font-size: 12px;
  margin-bottom: 7px;
}

.btn_analysis {
  width: 423px;
/*  outline: 2px solid blue;*/
  display: flex;
  justify-content: space-between;


}

.btn_analysis_left,
.btn_analysis_right {
  width: 91px;
/*  height: 36px;*/
  color: #0098EA;
  font-weight: 400;
  font-size: 16px;
  border-radius: 18px;
  border: 1px solid #0098EA;
  
}

.btn_arrow_left {
  background: url(../img/arrow_back_black_24dp 1.svg);
  background-position: left;
  background-repeat: no-repeat;
 
}

.btn_arrow_right {
  background: url(../img/arrow.svg);
  background-position: right;
  background-repeat: no-repeat;


}
	

</style>