
  
  <body id="body" style="transform:translateY(0px)">
  <p>1</p>
  <p>2</p>
  <p>3</p>
  <p>4</p>
  <p>5</p>
  <p>6</p>
  <p>7</p>
  <p>8</p>
  <p>9</p>
  <p>10</p>
  <p>11</p>
  <p>12</p>
  <p>13</p>
  <p>14</p>
  <p>15</p>
  <p>16</p>
  <p>17</p>
  <p>18</p>
  <p>19</p>
  <p>20</p>
</body>
<script>
  document.addEventListener("wheel", function (e) {

    // get the old value of the translation (there has to be an easier way than this)
    var oldVal = parseInt(document.getElementById("body").style.transform.replace("translateY(","").replace("px)",""));

    // to make it work on IE or Chrome
    var variation = parseInt(e.deltaY);
    
    // update the body translation to simulate a scroll
    document.getElementById("body").style.transform = "translateY(" + (oldVal - variation) + "px)";

    return false;
    
}, true);
  </script>
  <style>
  body {
    overflow-y:hidden;
    overflow-x:hidden;
}
  </style>
  
