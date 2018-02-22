<template>
<section id="programme">
  <div class="container">
    <h2 class="programme-header">주로 이런걸 해요!</h2>
    
    <div class="card-floor">
      <div class="row">
        <div class="col-md-4">
          <div class="card">
            <img class="card-img-top" src="../assets/programme/git-back.jpg" alt="" width="100%" height="190">
            <div class="card-body">
              <h5 class="card-title">Git & Github</h5>
              <p class="card-text">협업 프로젝트를 위한 Git, Github를 살펴봐요!</p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card">
            <img class="card-img-top" src="../assets/programme/designpattern-back.png" alt="" width="100%" height="190">
            <div class="card-body">
              <h5 class="card-title">디자인 패턴</h5>
              <p class="card-text">효율적인 코딩을 위해 나타난 여러 디자인 패턴을 알아봅니다!</p>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card">
            <img class="card-img-top" src="../assets/programme/hackathon-back.png" alt="" width="100%" height="190">
            <div class="card-body">
              <h5 class="card-title">각종 대회</h5>
              <p class="card-text">해커톤, 알고리즘 대회, 교내 경진대회의 적극적인 참여를 추천해요!</p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="card-floor">
      <div class="row">
        <div class="col-md-6">
          <div class="card">
            <img class="card-img-top" src="../assets/programme/latest-1-back.jpg" alt="" width="100%" height="190">
            <div class="card-body">
              <h5 class="card-title">최신 기술스택</h5>
              <p class="card-text">정신없이 쏟아져 나오는 최신 기술들.. 중요 키워드를 통해 핵심적인 내용을 캐치해요! </p>
            </div>
          </div>
        </div>
        <div class="col-md-6">
          <div class="card">
            <img class="card-img-top" src="../assets/programme/sharing-back.jpg" alt="" width="100%" height="190">
            <div class="card-body">
              <h5 class="card-title">다양한 정보공유</h5>
              <p class="card-text">컨퍼런스 및 세미나 행사, 오픈소스 경험, 학습 사이트, 검색 팁 등 다양한 정보를 공유하며 서로 도움을 주고 받아요!</p>
            </div>
          </div>                            
        </div>
      </div>
    </div>

    <h4 class="programme-footer">#세미나는 한 달에 한번씩 진행</h4>

  </div>
</section>
</template>

<script>
export default {
  name: 'Programme',
  data () {
    return {
      tmp: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#programme {
  padding-top: 8vh;
  padding-bottom: 8vh;
}
.programme-header {
  padding-top: 30px;
  padding-left: 10px;
}
.programme-footer {
  margin-top: 20px;
  padding-left: 10px;
  color: #42b983;
}

.card-floor {
  width: 100%;
}
.card {
  position: relative;
  margin-top: 15px;
  border: none;

  background: #ffff6d; /* Old browsers */
  background: -moz-linear-gradient(45deg, #ffff6d 0%, #ffff87 100%); /* FF3.6-15 */
  background: -webkit-linear-gradient(45deg, #ffff6d 0%,#ffff87 100%); /* Chrome10-25,Safari5.1-6 */
  background: linear-gradient(45deg, #ffff6d 0%,#ffff87 100%); /* W3C, IE10+, FF16+, Chrome26+, Opera12+, Safari7+ */
  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#ffff6d', endColorstr='#ffff87',GradientType=1 ); /* IE6-9 fallback on horizontal gradient */
}
.card::before {
  z-index: -1;
  position: absolute;
  content: "";
  bottom: 15px;
  left: 10px;
  width: 50%;
  top: 80%;
  max-width:300px;
  background: #777;
  -webkit-box-shadow: 0 15px 10px #777;
  -moz-box-shadow: 0 15px 10px #777;
  box-shadow: 0 15px 10px #777;
  -webkit-transform: rotate(-3deg);
  -moz-transform: rotate(-3deg);
  -o-transform: rotate(-3deg);
  -ms-transform: rotate(-3deg);
  transform: rotate(-3deg);
}
.card-body {
  color: #000;
  opacity: 0.7;
}
.card-title {
  font-weight: 600;
}
</style>
