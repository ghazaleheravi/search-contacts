# search-contacts
<!doctype html>
<html>
<head>
   <meta lang="en-us" dir="ltr">
   <title>search</title>

</head>

<body>
    <div>
       <label for="search">Search by contact name:</label> 
       <input id="search" type="text">
       <button>Search</button>
    </div>

    <p></p>

    <script>

        let name = document.querySelector('#search');
        let button = document.querySelector('button');
        let number = document.querySelector('p'); 

        button.addEventListener('click',search);
        
        function search(){
           let names = ['ghazaleh','reza','armin'];  
           let numbers = [5699252,5759252,7031563];
           let result;
           let searchName = name.value.toLowerCase();

           name.value = '';
           name.focus();
          
           for(let i=0;i<names.length;i++){
            if(searchName === names[i]){
              number.textContent = `${names[i]} : ${numbers[i]}`;
              break;
             }else {
                 number.textContent = 'Contact not found.';
             }
            }
         
        }

      </script>
</body>
</html>




        



        


        











    </script>
</body>



</html>
