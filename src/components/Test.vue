<template>
<div id="ubercontainer">
  <div id="in-container">
    <span class="static second">We always wonder</span>
    <span class="the-second"></span>
  </div>
</div>
</template>

<script>
export default {
  name: 'Test',
  mounted: function() {
    var second =  [ 'Flow', 'Architecture', 'Optimizing', 'Latest Technology Stack', 'Open Source'];
    var secondM = [];
    var positions = [];
    var el;
    var secondEl = $('.the-second');
    var container = $('#in-container');

    secondEl.text(second[0]);
    for(var i=0; i<second.length; i++) {
      el = $('<span class="measurable">' + second[i] + '</span>');
      container.append(el);
      secondM.push(el.width());
      el.css({
        position: 'absolute',
        visibility: 'hidden'
      })
    }

    $('#in-container > span').each(function() {
      positions.push($(this).position());
    });
    $('#in-container > span').each(function() {
      var pos = positions.shift(); // ??
      $(this).css({
        position: 'absolute',
        left: pos.left,
        top: pos.top
      });
    });

    var secondInitialWidth = secondEl.width();

    var activeWordsIndex = 0;
    setInterval(function() {
      activeWordsIndex++;
      var secondIndex = activeWordsIndex % second.length;
      secondEl.text(second[secondIndex]);

      var secondLineOffset = (secondM[secondIndex] - secondInitialWidth) / 2; // ??

      $('.static.second').css({
        transform: 'translateX(' + (-secondLineOffset) + 'px)'
      });

      secondEl.css({
        transition: 'none',
        transform: 'translate(' + (-secondLineOffset) + 'px, 30px)',
        opacity: '0'
      });
      setTimeout(function() {
        secondEl.css({
          transition: 'all 1s ease',
          transform: 'translate(' + (-secondLineOffset) + 'px, 0px)',
          opacity: '1'
        });
      }, 50)
    }, 2000)
  },
}
</script>

<style scoped>
#ubercontainer {
    width: 100%;
    margin: 10px auto;
    padding: 30px 0;
}
#in-container {
    position: relative;
    text-align: center;
    font-family: sans-serif;
    font-size: 32px;
    font-weight: 800;
    color: #4a6b82;
    width: 100%;
    height: 78px;
}
.measurable {
  position: absolute;
  visibility: hidden;
}
.static.second {
    padding-right: 6px;
    transition: transform 1s ease;
}
.the-second {
  color: #42b983;
}

@media (max-width: 768px) {
  #in-container {
    font-size: 16px;
  }
}
</style>