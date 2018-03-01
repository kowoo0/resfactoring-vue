<template>
<nav class="navbar fixed-top navbar-expand-md navbar-light bg-light">
    <a class="navbar-brand" href="#intro" @click="jumpToHome">
        <img src="../assets/brand/resfactoring_icon.svg" width="32" height="32" alt="" />    
        <span class="brand-name d-inline-block align-middle">리스펙토링</span>
    </a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbar-collapse">
        <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbar-collapse">
        <ul class="navbar-nav">
            <li class="hidden active">
                <a href="#intro"></a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#about" @click="jumpToSection">{{ about | upper }}</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#programme" @click="jumpToSection">{{ programme | upper }}</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#activity" @click="jumpToSection">{{ activity | upper }}</a>
            </li>
            <li class="nav-item">
                <a class="nav-link" href="#apply" @click="jumpToSection">{{ apply | upper }}</a>
            </li>
        </ul>
    </div>
</nav>
</template>

<script>
export default {
  name: 'Nav',
  mounted: function() {
    var _this = this,
        lastId,
        navBar = $('.navbar-nav'),
        navBarHeight = $('.navbar').outerHeight(),
        // All list items
        menuItems = navBar.find('a'),
        // Anchors corresponding to menu items
        scrollItems = menuItems.map(function(){
            var item = $($(this).attr("href"));
            if (item.length) { return item; }
        });


    $(window).scroll(function() {
        // Get container scroll position
        var fromTop = $(this).scrollTop();
    
        // Get id of current scroll item
        var cur = scrollItems.map(function(){
            if ($(this).offset().top <= fromTop + 2)
            return this;
        });
        // Get the id of the current element
        cur = cur[cur.length-1];
        var id = cur && cur.length ? cur[0].id : "";

        if (lastId !== id) {
            lastId = id;
            // Set/remove active class
            menuItems
                .parent().removeClass("active")
                .end().filter("[href='#"+id+"']").parent().addClass("active");
        }  
    });
  },
  data () {
    return {
        about: 'about',
        programme: 'programme',
        activity: 'activity',
        apply: 'apply'
    }
  },
  methods: {
    jumpToHome: function(e) {
        e.preventDefault();

        $('html, body').animate({scrollTop: 0}, 600);
    },
    jumpToSection: function(e) {
        e.preventDefault();

        var target = e.target,
            type = target.innerText.toLowerCase(),
            el = $('#' + type),
            offset = el.offset();         

        $('html, body').stop().animate({scrollTop: offset.top}, 600);
    }
  },
  filters: {
    upper: function(value) {
        if(!value) return ''
        value = value.toString()
        return value.toUpperCase()
    },
    capitalize: function (value) {
        if (!value) return ''
        value = value.toString()
        return value.charAt(0).toUpperCase() + value.slice(1)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.navbar {
    box-shadow: 0 0 1px rgba(0,0,0,0.25);
}
.navbar-nav {
    width: 100%;
}
.navbar-light .navbar-nav .active>.nav-link { color: #42b983; }
.brand-name {
    font-size: 1.2rem;
    font-weight: 600;
    color: #2c3e50;
}
</style>
