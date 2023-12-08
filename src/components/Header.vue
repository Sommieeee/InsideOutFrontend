<template>
  <nav>
    
    <div class="nav-inner">
           <!-- Logo -->
         <div class="logo">
            <img src="@/assets/images/logo.png" alt="" />
         </div>
          <!-- Links -->
          <div class="links">
            <a href="#">What's New</a>
            <a href="#">Shop</a>
            <a href="#">Brands</a>
            <a href="#">Blog</a>
            <a href="#">Contact</a>
          </div>
       
           <!-- Icons -->
           <div class="box">
            <input type="text" v-model="search" placeholder="Search for Brands">
           </div>
           <div class="icons">
            
            <span class="icon">
              <svg width="20" height="46" viewBox="0 0 51 46" fill="none" xmlns="http://www.w3.org/2000/svg">
              <g clip-path="url(#clip0_73_66)">
              <path d="M38.25 11.5H34C34 7.26415 30.1963 3.83331 25.5 3.83331C20.8037 3.83331 17 7.26415 17 11.5H12.75C10.4125 11.5 8.5 13.225 8.5 15.3333V38.3333C8.5 40.4416 10.4125 42.1666 12.75 42.1666H38.25C40.5875 42.1666 42.5 40.4416 42.5 38.3333V15.3333C42.5 13.225 40.5875 11.5 38.25 11.5ZM25.5 7.66665C27.8375 7.66665 29.75 9.39165 29.75 11.5H21.25C21.25 9.39165 23.1625 7.66665 25.5 7.66665ZM38.25 38.3333H12.75V15.3333H17V19.1666C17 20.2208 17.9562 21.0833 19.125 21.0833C20.2938 21.0833 21.25 20.2208 21.25 19.1666V15.3333H29.75V19.1666C29.75 20.2208 30.7062 21.0833 31.875 21.0833C33.0438 21.0833 34 20.2208 34 19.1666V15.3333H38.25V38.3333Z" fill="#697F94"/>
          </g>
          <defs>
          <clipPath id="clip0_73_66">
          <rect width="51" height="46" fill="white"/>
          </clipPath>
          </defs>
          </svg>
          <span class="icon">
                          <svg width="20" height="53" viewBox="0 0 49 40" fill="none" xmlns="http://www.w3.org/2000/svg">
            <g clip-path="url(#clip0_73_59)">
            <path d="M29 13.25C31.6583 13.25 33.8333 15.2375 33.8333 17.6666C33.8333 20.0958 31.6583 22.0833 29 22.0833C26.3417 22.0833 24.1667 20.0958 24.1667 17.6666C24.1667 15.2375 26.3417 13.25 29 13.25ZM29 35.3333C35.525 35.3333 43.0167 38.1821 43.5 39.75H14.5C15.0558 38.16 22.4992 35.3333 29 35.3333ZM29 8.83331C23.6592 8.83331 19.3333 12.7862 19.3333 17.6666C19.3333 22.5471 23.6592 26.5 29 26.5C34.3408 26.5 38.6667 22.5471 38.6667 17.6666C38.6667 12.7862 34.3408 8.83331 29 8.83331ZM29 30.9166C22.5475 30.9166 9.66667 33.8758 9.66667 39.75V44.1666H48.3333V39.75C48.3333 33.8758 35.4525 30.9166 29 30.9166Z" fill="#697F94"/>
            </g>
            <defs>
            <clipPath id="clip0_73_59">
            <rect width="58" height="53" fill="white"/>
            </clipPath>
            </defs>
            </svg>
              </span>
            </span>
            
           </div>
    </div>
  </nav>
</template>

<script>
export default{
  data(){
    return{
      search: ""
    }
  }
}
</script>

<style scoped>
nav{
  border-bottom: 2px solid #f8f8f8;
}
nav .nav-inner{
  height: 90px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  max-width: calc(1440px - 170px);
  width: 100%;
  margin: auto;


}

.nav-inner .links a{
  margin: 0px 16px;
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 16px;
  color: #697F94;
  border-bottom: 1px solid transparent;
  transition: .3s;
  text-decoration-line: none;
}

.nav-inner .links a:hover{
  border-color: #697F94;
}

.icons span{
  margin: 0 13px;
  display: inline-block;
  color: #697F94;
 
}
input {
  display: block;
  width: 400px;
  margin: 20px auto;
  padding: 10px 45px;
  background-size: 15px 15px;
  font-size: 16px;
  border: none;
  border-radius: 5px;
  box-shadow: rgba(50, 50, 93, 0.13) 0px 2px 5px -1px,
    rgba(0, 0, 0, 0.3) 0px 1px 3px -1px;
  
}
::placeholder {
  color: #697F94;
  opacity: 1; 
  font-size: 14px;
  
}

</style>