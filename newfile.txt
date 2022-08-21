var hr_number = document.getElementById('hr');
var min_number = document.getElementById('min');
var sec_number = document.getElementById('sec');
var clock = setInterval(myclock,1000);
function myclock(){
    var time = new Date();
    hr_number.innerText = time.getHours()%12;
    hr_number.style.color='green';
    hr_number.style.fontSize = '4em';
    hr_number.style.textAlign = 'center';  
    hr_number.style.textShadow = '2px 2px 3px rgb(37, 138, 133)';  
    min_number.innerText = time.getMinutes();
    min_number.style.fontSize = '4em';
    min_number.style.color='green';
    min_number.style.textAlign = 'center';
    min_number.style.textShadow = '2px 2px 3px rgb(37, 138, 133)'
    sec_number.innerText = time.getSeconds();
    sec_number.style.fontSize = '4em';
    sec_number.style.color='green';
    sec_number.style.textAlign = 'center';
    sec_number.style.textShadow = '2px 2px 3px rgb(37, 138, 133)'
}
