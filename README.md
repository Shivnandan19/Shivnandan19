body{
    margin: 0;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background-image: linear-gradient(
        to bottom,
        #dcdcdc 50%,
        #e9e9e9 50%
    );
    font-family: sans-serif;
}


*{
    margin: 0;
    padding: 0;
}

main{
    width: 300px;
    height: max-content;
    min-height: 300px;
    background-color: white;
    border-radius: 30px;
    padding:20px 20px;
    box-shadow: 0 30px 50px #5553;
    box-sizing: border-box;
}

main form{
    border: 1px solid #5553;
    display: flex;
    justify-content: space-between;
    border-radius: 30px;
}

/* search bar */
main form input,
main form button{
    border: none;
    background-color: transparent;
    outline: none;
    padding: 10px;
}

main form i{
    opacity: 0.7;
}

main .result{
    padding: 20px;
    text-align: center;
}
main .result .name{
    font-weight: bold;
    font-size: large;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
}

main .temperature img{
    width: 150px;
    filter: drop-shadow(
        0 10px 50px #000
    );
}

main .temperature figcaption{
    font-size: 3em;

}

main .description{
    padding: 10px 0 30px;
}

main ul{
    list-style: none;
    display:grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 10px;
}

main li{
    background-color: #f78a55;
    color: #fff;
    border-radius: 10px;
    padding: 20px 10px;
    background-image: linear-gradient(
        to bottom,
        transparent 50%,
        #0003 50%
    );
    font-weight: bold;
    font-size: small;
}

main li i{
    font-size: 2rem;
    display: block!important;
    margin: 20px 0;

}

main li:nth-child(2){
    background-color: #b56291;
}

main li:nth-child(3){
    background-color: #48567b;
}

main.error{
    animation: errorEffect 0.3s linear 1;
}

@keyframes errorEffect{
    0%{
        transform: translate(10px , 5px);
    }
    25%{
        transform: translate(-5px, 0);
    }

    50%{
        transform: translate(8px, 2px);

    }
    75%{
        transform: translate(-2px, 5px);

    }
    100%{
        transform: translate(0, 0);

    }
}
