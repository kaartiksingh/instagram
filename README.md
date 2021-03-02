# instagram
 {
  margin: 0;
  padding: 0;
  outline: none;
}
body {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
}
#check {
  -webkit-appearance: none;
  display: none;
}
#searchbox {
  width: 0px;
  height: 55px;
  border-radius: 50px;
  border: none;
  background: #000;
  color: #fff;
  font-size: 25px;
  transition: 0.3s ease;
  transform: scale(0);
}
input[type="search"] {
  padding: 0 25px;
}
#searchbox::placeholder {
  font-style: italic;
}
span {
  background: #0048ff;
  padding: 25px;
  border-radius: 50%;
  font-size: 20px;
  color: #fff;
  transition: 0.3s ease;
  margin-right: 40px;
}
#check:checked ~ label #searchbox {
  width: 350px;
  transform: scale(1);
  border: 3px solid #fff;
}
#check:checked ~ label span {
  color: #000;
  background: #fff;
  position: relative;
  margin-left: 5px;
}
section {
  height: 1px;
  width: 1px;
  box-shadow: 0 0 0 0 #0048ff;
  position: absolute;
  transition: 0.6s ease;
  border-radius: 50%;
}
#check:checked ~ section {
  box-shadow: 0 0 0 3500px #0048ff;
}
label {
  z-index: 1;
  width: 100%;
  display: flex;
  justify-content: center;
  flex-wrap: nowrap;
  overflow: hidden;
}
/*This is my youtube channel link*/
a {
  position: absolute;
  bottom: 20px;
  font-weight: 600;
  text-decoration: none;
  font-size: 20px;
  font-family: sans-serif;
  right: 20px;
  color: #000;
}
a:hover {
  color: red;
}
