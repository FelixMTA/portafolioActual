

<div class="container">

    <div class="row">
        <div class="col">
         1

        </div>
        <div class="col">
            2
        </div>
        <div class="col">
3
        </div>
    </div>
</div>




<style>
    .row{
width: 100%;
height: 100%;
    }
    img{ 
        border-radius: 50%;
        width: 50px;
        height: 50px;
       
       

    }
    .col{
        display: flex;
        justify-content: end ;
        align-items: flex-end;
        text-align: end;
        
        width: 100%;
        height: 100%;
        animation: arriba 2s infinite;
    }
    @keyframes arriba {
       
        0% {transform: translateY(0);}
        
        100% {transform: translateY(100);}
    }
</style>