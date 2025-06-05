 <script>
      const Userusername = document.getElementById('username');
      const Userpassword = document.getElementById('password');
      const submitbutton = document.getElementById('Submit');
      submit.onclick = function() {
        const response = axios.post('https://abhirebackend.onrender.com/auth/login',{
        Userusername,Userpassword
        },{
          headers:{
            'Content-Type' : 'application/json'
          }
        });
        console.log(response.data);
      }

     </script>
