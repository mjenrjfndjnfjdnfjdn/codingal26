<html>
  <body>
    <h2>------</h2>
    <p>-------</p>
    <p>-------</p>
    <p id="details"</p>
    <script>
      class Car {
        constructor(brand) {
          this.carname = brand;
        }
        present() {
          return "I Want To One Day Own A " + this.carname;
        }
      }
      class Model extends Car {
        constructor(brand, mod) {
          super(brand);
          this.model = mod;
        }
        show() {
          return this.present() + ", It Is The " + this.model + " Version";
        }
      }
      let myCar = new Model("Lamborghini", "Aventador");
      document.getElementById("details").innerHTML = myCar.show();
    </script>
  </body>
</html>
