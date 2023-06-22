<template>
    <header>
        <div class="logo">
            <img src="assets/images/logoVest.png" alt="">
        </div>
        <nav>
            <ul class="list-menu">
                <li><a href="#home">home</a></li>
                <li><a href="#serviço">servico</a></li>
                <li><a href="#sobre">sobre</a></li>
                <li><a href="#protifolio">portifolio</a></li>
                <li><a href="#princig">princing</a></li>
                <li><a href="#contato">contato</a></li>
                <ul>
                    <li><a class="#"><i class="fa-solid fa-user"></i></a></li>
                    <li><a class="#"><i class="fa-solid fa-user"></i></a></li>
                </ul>
            </ul>
        </nav>
        
    </header>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    header{
        display: flex;
        align-items: center;
        justify-content: space-around;
        padding: 10px;
        background-color: transparent;
    }header .logo{
        display: inline-table;
        padding: 10px;
    }header h1{
        text-align: center;
        color: #ef0a0a;
        font-size: 2.5rem;
    }header .text-logo{
        padding: 0 10px;
        font-size: 1.5rem;
        text-align: center;
        color: #ef0a0a;
    }.list-menu{
        display: flex;
        align-items: center;
        gap: 15px;
    }.list-menu li a{
        text-decoration: none;
        color: #ef0a0a;
        width: 0;
        height: 0;
        font-size: 1.3rem;
        text-transform: capitalize;
    }.list-menu li a::after{
        content: '';
        width: 0;
        height: 0;
        display: block;
        text-decoration: none;
        border-bottom: 2px solid transparent;
        transition: .9s;
    }.list-menu li a:hover::after{
        text-decoration: none;
        width: 100%;
        height: 0;
        padding: 0;
        border-bottom: 2px solid #ef0a0a;
    }
</style>
