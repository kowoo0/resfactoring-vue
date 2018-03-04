<template>
<section id="apply">
  <div class="apply-body">
    <div class="container-fluid">
      <div class="apply-txt">
        <h1 class="apply-date">2기 모집기간</h1>
        <h1 class="apply-date">3월 5일 ~ 3월 14일</h1>
        <div class="apply-box-cover">
          <a class="apply-box" :href="applyLink" target="_blank">
            <div class="apply-box-frame">
              <span class="apply-box-txt">지원하기</span>
            </div>
          </a>
          <a class="apply-box" :href="inquiryLink" target="_blank">
            <div class="apply-box-frame">
              <span class="apply-box-txt">카톡문의</span>
            </div>
          </a>
        </div>
        <h2 class="apply-sub">개발이 재밌고 함께 성장하는 것에 가치를 느끼시는 분,
           자신의 소스를 오픈하는 '오픈소스' 개발에 관심있으신 분, 나는 개발자다! 부족하지만 열정이 넘치는 36학생 개발자의 많은 지원부탁드립니다!</h2>
      </div>
    </div>
  </div>
</section>
</template>

<script>
export default {
  name: 'Apply',
  data () {
    return {
      applyLink: 'https://docs.google.com/forms/d/e/1FAIpQLSdP1I0RaZ9ViLgoTo-6j-2DACiTPwNpQRynS-tcMpRkmAx_2w/viewform?usp=sf_link/',
      inquiryLink: 'https://open.kakao.com/o/slHWnrI/'
    };
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#apply {
  display: table;
  padding: 80px 0px;
  width: 100%;
  height: 100vh;

  background: url(../assets/apply/apply-back.jpeg);
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
.apply-body {
  display: table-cell;
  vertical-align: middle;
}
.apply-box-cover {
  width: 100%; height: 200px;

    /* Center slide text vertically */
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center;   
}
.apply-box {
  display: block;
  padding: 15px;
  width: 50%; height: 150px;
  color: #fff;
}
.apply-box:hover .apply-box-frame {
  transform: scale(1.1);
}
.apply-box:hover .apply-box-frame::before {
  display: block;
}
.apply-box:nth-of-type(1) {
  background: rgb(123,104,238); /* Old browsers */
  background: -moz-linear-gradient(-45deg, rgb(123,104,238) 0%, rgb(229,229,229) 100%); /* FF3.6-15 */
  background: -webkit-linear-gradient(-45deg, rgb(123,104,238) 0%,rgb(229,229,229) 100%); /* Chrome10-25,Safari5.1-6 */
  background: linear-gradient(135deg, rgb(123,104,238) 0%,rgb(229,229,229) 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#7b68ee', endColorstr='#e5e5e5',GradientType=1 ); /* IE6-9 fallback on horizontal gradient */
}
.apply-box:nth-of-type(2) {
  background: rgb(0,191,255); /* Old browsers */
  background: -moz-linear-gradient(-45deg, rgb(0,191,255) 0%, rgb(229,229,229) 100%); /* FF3.6-15 */
  background: -webkit-linear-gradient(-45deg, rgb(0,191,255) 0%,rgb(229,229,229) 100%); /* Chrome10-25,Safari5.1-6 */
  background: linear-gradient(135deg, rgb(0,191,255) 0%,rgb(229,229,229) 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#00bfff', endColorstr='#e5e5e5',GradientType=1 ); /* IE6-9 fallback on horizontal gradient */
}
.apply-box-frame {
  width: 100%; height: 100%;
  /* border: 1px solid #fff; */
  padding: 30px 15px;

  text-align: left;
  transition: all .2s ease-in-out;
}
.apply-box-txt {
  font-size: 31px;
  font-family: 'Nanum Pen Script', cursive;  
  font-weight: 700;
  opacity: 0.9;
}
.apply-txt {
  text-align: center;
}
.apply-date {
  margin-bottom: 10px;
  padding: 0 12px;

  font-family: 'Nanum Pen Script', cursive;
}
.apply-sub {
  padding: 12px 20px;
  font-family: 'Nanum Pen Script', cursive;  
}

.container-fluid { padding: 0; }

/* Medium devices (tablets, 768px and up) */
@media (min-width: 768px) { 
  .apply-box-cover {
    margin-top: 80px;
    margin-bottom: 80px;
    padding-left: 200px;
    padding-right: 200px;
  }
  .apply-box {
    width: 200px;
    height: 200px;

    -webkit-box-shadow: 0 8px 6px -6px black;
	   -moz-box-shadow: 0 8px 6px -6px black;
	        box-shadow: 0 8px 6px -6px black;
  }
  .apply-box:nth-of-type(2) {
    margin-left: 50px;
  }
  .apply-sub {
    padding: 12px 60px;
  }
}
</style>
