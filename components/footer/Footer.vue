<template>
  <div class="footer">
   
       <nav>
        <ul>
          <li>
            <a href="https://sqoin.us/coin/">
              Sqoin
            </a>
          </li>
        
          <li>
            <a href="https:///blog.creative-tim.com">
              SQoin Galerie
            </a>
          </li>
        </ul>
      </nav>
      <div class="copyright">
        &copy; {{ year }}, Created and Coded by
        
        <a href="https://sqoin.us/coin/" target="_blank" rel="noopener"
          >Sqoin TEAM</a
        >.
      </div></div>
</template>

<script>
export default {
  name: 'VmFooter',

  props: {
    backgroundColor: String,
    type: String
  },
  data() {
    return {
      year: new Date().getFullYear()
    };
  }
};
</script>

<style lang="scss" scoped>
     
 .copyright{float:right;}
 .footer{
    height:50px;
    background: black;
    color: white;
    padding: 24px 0;

    

    nav{
        display: inline-block;
        float: left;
    }

    ul{
        margin-bottom: 0;
        padding: 0;
        list-style: none;

        li{
            display: inline-block;

            a{
                color: orange;
                
                text-transform: uppercase;
                text-decoration: none;

                &:hover{
                    text-decoration: none;
                }
            }
        }
    }

    

    &:after{
        display: table;
        clear: both;
        content: " ";
    }
}

 
</style>
