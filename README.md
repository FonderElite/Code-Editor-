# Full Code Here:
```html
<html>
<head>
<script src="https://cdnjs.cloudflare.com/ajax/libs/ace/1.4.12/ace.js"></script>
<link rel="shortcut icon" href="https://www.svgrepo.com/show/44984/atom.svg">
<link rel="https://cdn.jsdelivr.net/gh/warengonzaga/daisy.js/daisy.js">
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js" integrity="sha512-894YE6QWD5I59HgZOGReFYm4dnWc1Qt5NtvYSaNcOP+u1T9qYdvdihz0PPSiiqn/+/3e7Jo4EaG7TubfWGUrMQ==" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.js" integrity="sha512-n/4gHW3atM3QqRcbCn6ewmpxcLAHGaDjpEBu4xZd47N0W2oQ+6q7oc3PXstrJYXcbNU1OHdQ1T7pAP+gi5Yu8g==" crossorigin="anonymous"></script>
<script src="https://cdn.jsdelivr.net/gh/warengonzaga/daisy.js/daisy.min.js"></script>
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Poppins&display=swap" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/sweetalert2@10"></script>

<title>Atomic Editor</title>
<style>
#ul{
    display:none;
}
    #cosmic2{
        display: block;
        width: 24%;
        height:10%;
        position:absolute;     
        top:0%;
        left: 61.5%;
    }
    body{
        background-color: rgb(44, 43, 43);
    }
    /*Phone Resolution Goes Here*/
    *{
        color:white;
        font-family:'poppins';
    }
        #container-here{
            position: absolute;
            width: 100%;
            height: 100%;
            background-color:rgb(48, 46, 46);
          
        }
        #headerh1{
            position: absolute;
            top: -4%;
            height: 10%;
            width: 96%;
            font-size: 5vh;
            border: 1px solid white;
            padding: 15px;
            font-size: 5vh;
            text-shadow: 0px 0px 4px 5px black;
            font-weight: 1000;
            background-color:rgb(26, 25, 25);
            color: white;
            
        }
        /*Done*/
        #cosmic{
            position:absolute;
            width: 25%;
            height: 10%;
            top: -1%;
        left:60%;
        z-index: 1;
        display:none;
        transition:0.2s;
        }
        #cosmic:hover{
            transition:0.5s;
            cursor: pointer;
            }
            /*Hamburger navbar*/
            ul{
                list-style: none;
                text-decoration: none;
                display:none;
               
            }
            a{
                text-decoration: none;
                color: white;
                border: 1px solid white;
                border-radius: 10%;
                padding: 5px 5px;
                background-color: rgb(53, 58, 59);
                text-shadow: 0px 6px 7px black;
                z-index:2;
                transition: 0.5s
            }
            #firstli{
                position: absolute;
                 top: 19%;
                    left: 35%;
                    padding: 1vh 2vh;
                    font-size: 2.5vh;
                    z-index:1;
                }
                #firstli:hover{
                  padding: 1vh 2vh;
                transition: 0.5s;
                }
                #secondli{
                    position: absolute;
                    left: 28%;
                    top: 30%;
                    padding: 1vh 2vh;
                    font-size: 2.5vh;
                    z-index:1;
                }
                #secondli:hover{
                    padding: 1vh 2vh;
                    transition: 0.5s
                }
                #thirdli{
                    position: absolute;
                    left: 36.5%;
                    top: 40%;
                    padding: 1vh 2vh;
                    font-size: 2.5vh;
                    z-index:1;
                }
                #thirdli:hover{
                    padding: 1vh 2vh;
                    transition: 0.5s;
                }
                #fourthli{
                    position: absolute;
                    left: 30%;
                    top: 50%;
                    padding: 1vh 2vh;
                     font-size: 2.5vh;
                    z-index:1;
                }
                #fourthli:hover{
                    padding: 1vh 2vh;
                    transition: 0.5s;
                }
                #cover{
                    width: 100%;
                    height: 105%;
                    background-color: rgb(29, 29, 29);
                    opacity: 0.9;
                    position: fixed;
                    top: -5%;
                    z-index: 1;
                    display: none;

                }
                .layer{
                    position: fixed;
                    background-color: whitesmoke;
                }
                #layer1{
                    width: 10%;
                    height: 0.5%;
                    top: 1.6%;
                    left: 86%;
                    border: 1px solid white;
                    z-index: 2;
                    border-radius: 10px;
                }
                #layer2{
                    width: 10%;
                    height: 0.5%;
                    top: 3.9%;
                    left: 86%;
                    border: 1px solid white;
                    z-index: 2;
                    border-radius: 10px;
                }
                #layer3{
                    width: 10%;
                    height: 0.5%;
                    top: 6%;
                    left: 86%;
                    border: 1px solid white;
                    z-index: 2;
                    border-radius: 10px;
                }
           
           /*Hamburger navbar end*/
           #codelogo{
            position: absolute;
            width: 5%;
            height: 10%;
            top: 1%;
            left: 93%;
            display: none;
        }
        #codee{
           position: absolute;
           top: 14.5%;
           width: 52%;
           height: 90%;
           overflow: scroll;

           
        }

@media(min-width: 1000px){
    body{
        margin:0;
        padding: 0;
        color:white;
        font-family:'poppins';
        background:black;
        height: 98%;
        width: 100%;

        
        }
#container-here{
    position: absolute;
    width: 100%;
    height: 100%;
    background-color:rgb(48, 46, 46);
}
#headerh1{
    position: absolute;
    top: -3%;
    height: 10%;
    width: 99%;
    font-size: 5vh;
    border: 1px solid white;
    padding: 15px;
    font-size: 6vh;
    text-shadow: 0px 0px 4px 5px black;
    font-weight: 1000;
    background-color:rgb(26, 25, 25);
    
}
#cosmic2{
    display: none;
}
#cosmic{
    position:absolute;
    width: 13%;
    height: 17%;
    top: -1.5%;
left:20%;
z-index: 1;
transition:0.2s;
display:block;
}
#cosmic:hover{
transition:0.5s;
cursor: pointer;
}
ul{
    list-style: none;
    text-decoration: none;
   display:block;
}
a{
    text-decoration: none;
    color: white;
    border: 1px solid white;
    border-radius: 10%;
    padding: 5px 5px;
    background-color: rgb(13, 122, 150);
    text-shadow: 0px 6px 7px black;
    z-index:2;
    transition: 0.5s

}

#firstli{
position: absolute;
    top: 3.5%;
    left: 40%;
    padding: 10px 15px;
}
#firstli:hover{
    padding: 15px 18px;
    transition: 0.5s;
}
#secondli{
    position: absolute;
    left: 51%;
    top: 3.5%;
    padding: 10px 15px;
}
#secondli:hover{
    padding: 15px 18px;
    transition: 0.5s;
}
#thirdli{
    position: absolute;
    left: 66%;
    top: 3.5%;
    padding: 10px 15px;
    
}
#thirdli:hover{
    padding: 15px 18px;
    transition: 0.5s;
}
#fourthli{
    position: absolute;
    left: 77%;
    top: 3.5%;
    padding: 10px 15px;
}
#fourthli:hover{
    padding: 15px 18px;
    transition: 0.5s;
}

#codelogo{
    position: absolute;
    width: 5%;
    height: 10%;
    top: 1%;
    left: 93%;
    display: block;
}
#codee{
   position: absolute;
   top: 14.5%;
   width: 52%;
   height: 90%;
   overflow: scroll;
   display: block;
   
}
.ace_editor .ace_marker-layer .ace_bracket { display: none }
/*Code editor Style*/

body { margin:0; padding:0; height:100%; width:100%; position: absolute;}
html{
    margin:0; 
    padding:0;
     height:120%;
      width:100%;
       position: absolute;
       background-color: white;

}

#editor {
    height: 90%;
    width:50%;
    display:inline-block;
    border: 1px solid white;
  
}

#down_container {
	height:80%;
	width:100%;
  white-space : nowrap; 
  overflow : hidden;
  position:absolute;
  top: 15%;
  left: 1%;
  

}

#iframe {
	height:90%;
	display:inline-block;
	width:50%;
    position:absolute;
    top:0%;
}

/* disable tag matching */
.ace_editor .ace_marker-layer .ace_bracket { display: none }

#chtheme{
    position: absolute;
    width: 7%;
    height: 10%;
    top: 2%;
    left: 31.5%;
    transition: 1s;
}
#chtheme:hover{
    cursor:pointer;
    transition: 1s;
    box-shadow: 0px 0px 7px 1px rgb(81, 83, 83);
}
#hamburger{
    display:none;
}
#cover{
    display:none;
}

}
/*0px-768px* Resolution*/

</style>
</head>
<body>
<div class="container" id="container-here" onload="load()">
<div id="header">
<img id="cosmic" onclick="atomic()" src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/React-icon.svg/1280px-React-icon.svg.png"><h1 id="headerh1">Atomic Editor</h1>
<img id="cosmic2" src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/React-icon.svg/1280px-React-icon.svg.png">
<div id="hamburger">
    <div class="layer" id="layer1"></div>
    <div class="layer" id="layer2"></div>
    <div class="layer" id="layer3"></div>
</div>
<div id="cover">

</div>
<ul>
    <li><a id="firstli" href="#">MainPage</a></li>
    <li><a id="secondli" href="#">Documentations</a></li>
    <li><a id="thirdli" href="#">Liscense</a></li>
    <li><a  id="fourthli" href="#">StackOverFlow</a></li>
</ul>
<ul id="ul">
    <li><a id="firstli1" href="#">MainPage</a></li>
    <li><a id="secondli2" href="#">Documentations</a></li>
    <li><a id="thirdli3" href="#">Liscense</a></li>
    <li><a  id="fourthli4" href="#">StackOverFlow</a></li>
</ul>
<img id="codelogo" src="https://cdn.iconscout.com/icon/free/png-256/code-336-830581.png">
<img id="chtheme" src="https://cdn.iconscout.com/icon/premium/png-256-thumb/paintbrush-31-691605.png">
</div>
<div id='down_container'>

    <div id="editor">
    </div>
  
    <iframe id='iframe' frameBorder="0">
    </iframe>
  </div>
  
</div>
<script>
    $("#cosmic2").click(function(){
    
    logo =  $("#cosmic2").attr('src','https://media4.giphy.com/media/eNAsjO55tPbgaor7ma/giphy.gif').css({
          width: '17%',
          height:'9%',
          position:'absolute',
          top:'0%',
          left: '63%',
      })
      });
$(document).ready(function(){
$("#container-here").daisyjs({
    dotColor: 'cyan',
    lineColor: 'grey'
});

});
$("#cosmic").click(function(){
    
    logo =  $("#cosmic").attr('src','https://media4.giphy.com/media/eNAsjO55tPbgaor7ma/giphy.gif').css({
          width: '10%',
          height:'15%',
          position:'absolute',
          top:'0%',
          left: '21.5%'
      })
      });
function update()
{
	let idoc = document.getElementById('iframe').contentWindow.document;
	idoc.open();
	idoc.write(editor.getValue());
	idoc.close();
}


function setupEditor()
{
 window.editor = ace.edit("editor");
theme = editor.setTheme("ace/theme/monokai");
  editor.getSession().setMode("ace/mode/html");
  editor.setValue(`<!DOCTYPE html>
  <!--Made By FonderElite
    GitHub:https://github.com/FonderElite-->
<html>
<head>
    <style>

    </style>
</head>
<body>
</body>

</html>`,1); //1 = moves cursor to end

  editor.getSession().on('change', function() {
    update();
  });

  editor.focus();
  
  
  editor.setOptions({
    fontSize: "12pt",
    showLineNumbers: false,
    showGutter: false,
    vScrollBarAlwaysVisible:true,
    enableBasicAutocompletion: false, enableLiveAutocompletion: false
  });

  editor.setShowPrintMargin(true);
  editor.setBehavioursEnabled(false);
  
}


setupEditor();
update();


const changeTheme = $("#chtheme").click(function(){
    const codeThemes = ['monokai','cobalt','gob','terminal','chaos','ambiance','idle_fingers','iplastic'];
    let randomizedTheme = parseInt(Math.random() * codeThemes.length);
   // alert(randomizedTheme);
    switch(randomizedTheme){
case 0:
editor.setTheme(`ace/theme/${codeThemes[0]}`);
break;
case 1:
editor.setTheme(`ace/theme/${codeThemes[1]}`);
break;
case 2:
editor.setTheme(`ace/theme/${codeThemes[2]}`);
break;
case 3:
editor.setTheme(`ace/theme/${codeThemes[3]}`);
break;
case 4:
editor.setTheme(`ace/theme/${codeThemes[4]}`);
break;
case 5:
editor.setTheme(`ace/theme/${codeThemes[5]}`);
break;
case 6:
editor.setTheme(`ace/theme/${codeThemes[6]}`);
break;
case 7:
editor.setTheme(`ace/theme/${codeThemes[7]}`);
break;
    }
});
/*
const changeTheme = $("#chtheme").click(function(){
    const codeThemes = ['monokai','cobalt','gob','terminal','chaos','ambiance','idle_fingers','iplastic'];
  codeThemes.forEach(item =>{
      
  })
    
})
*/
const mobileHamburger = $('#hamburger').click(function(){
  let cover =   $('#cover').slideToggle(1000);
  let ul = $('ul');
  ul.slideToggle(400);
 first =  $('#firstli').css({
     backgroundColor: '#388E8E'
 })
 second =  $('#secondli').css({
    backgroundColor: '#2F4F4F'
 })
 third =  $('#thirdli').css({
    backgroundColor: '#2F4F4F'
 })
 fourth =  $('#fourthli').css({
    backgroundColor: '#2F4F4F'
 })
  let list = [
first,
second,
third,
fourth
  ]
})


</script>
</body>
</html>
```

