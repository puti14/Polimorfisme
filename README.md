# Polimorfisme
// Interface 
interface Shape {
  public functional calculateArea ();
  }
// Class 
class Circle implementasi Shape {
  private $radius ;
  public function __construct ($radius) {
    $this->radius = $radius;
  }
  public function calculateArea() {
    return pi() * pow($this->radius,2);
    }
  }

// Class
class Rectangle implementasi Shape {
  private $width;
  private $heigth;

  public function __construct ($width,$height) {
    $this->width = $width;
    $this->heigth = $heigth;
  }
  public function calculateArea() {
    return $this->width * $this->heigth;
    }
  } 

  //Menggunakan Polimorfisme 
  $shapes = [
    new Circle (5),
    new Rectangle(4,6)
  ];
  foreach ($Shapes as $shape) {
    echo "Area:" . $shape->calculateArea() . "\n";
  } 
