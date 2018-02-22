<template>
<section id="about">
  <div class="about-body">
    <div class="container">
      <div class="row">
        <div class="col-md-6">
          <div class="about-article">
            <h1 class="about-header">리펙은?</h1>
            <p><strong>안녕하세요!</strong> 36 개발자 커뮤니티 리스펙토링입니다!</p>
            <p>리펙은 멤버들이 학교 커리큘럼에서 얻기 힘든 <strong>정보를 공유</strong>하고, <strong>다양한 활동</strong>들을 통해 경험을 채워 좀 더 나은 개발자가 되는 것을 지향합니다.</p>              
            <p>이번에 <strong>2기 멤버</strong>를 새롭게 뽑고 있으며, 저번 1기 때의 부족한 점을 토대로 점차 좋은 모습을 갖춘 공식 동아리로 만들어나갈 수 있도록 노력하고 있습니다!!</p>
            <p>현재 컴퓨터학부 학생들을 위주로 모집하고 있으며 추후에는 타학과 학생들 또한 뽑을 예정입니다.</p>
            <p>2018년도 2기 리펙 멤버가 되어 다음 년도 <em>3기 멤버</em>들을 이끌어주세요!</p>
            <hr />
            <h5>Respect & Refactoring</h5>
          </div>
        </div>
        <div class="col-md-6">
          <div class="about-article">
            <div class="about-article-list">
              <div class="about-article-item">
                <img class="about-article-img" width="70" height="70" alt=""/>
                <div class="about-article-textbox">
                  <h5>열정</h5>
                  <h6 class="about-article-text">코딩에 관심만 있다면 누구나 참여가 가능해요</h6>
                </div>
              </div>
              <div class="about-article-item">
                <img class="about-article-img" src="../assets/about/teaming.png" width="70" height="70" alt=""/>
                <div class="about-article-textbox">
                  <h5>티밍</h5>
                  <h6 class="about-article-text">스터디, 협업 프로젝트, 외부 활동 등을 적극적으로 지원해요</h6>
                </div>
              </div>
              <div class="about-article-item">
                <img class="about-article-img" width="70" height="70" alt=""/>
                <div class="about-article-textbox">
                  <h5>경험</h5>
                  <h6 class="about-article-text">함께 배우기, 성장하기, 오픈소스로 기여하기 등으로 개발의 세계에 빠져들어요</h6>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
</template>

<script>
export default {
  name: 'About',
  data () {
    return {
      tmp: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#about {
  display: table;
  width: 100%;
  height: 100vh;
}
.about-body {
  display: table-cell;
  vertical-align: middle;
}
.about-article {
  padding: 16px 5px;
  width: 100%;
}
.about-article-list {

}
.about-article-item {
  display: grid;
  grid-template-columns: 25% 75%;

  margin-bottom: 10px;
}
.about-article-img {
  justify-self: center;
  align-self: center;

  padding: 10px;

  border: 1px solid #2c3e50;
  border-radius: 50%;
}
.about-article-textbox {
  align-self: center;

  padding: 14px 12px 14px 16px;

  text-align: left;
}
.about-header {
  margin-bottom: 30px;
}
.about-article-header { margin-bottom: 12px; }
.about-article-text { margin-bottom: 10px; font-weight: 500; color: darkgray; }

.col-md-6:nth-of-type(2) {
}
.col-md-6:nth-of-type(2) .about-article {
  height: 100%;
  display: table;
}
.col-md-6:nth-of-type(2) .about-article-list {
  display: table-cell;
  vertical-align: middle;
}
</style>
