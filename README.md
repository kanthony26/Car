public class Car {
	private int yearModel;
	private String make;
	private int speed;
	
	public Car(int year, String mk){
		yearModel = year;
		make = mk;
		speed = 0;
	}
	
	public static void main(String[] args) {
		Car mob = new Car(1976, "Caddy");
		mob.accelerate();
		System.out.println(mob.getSpeed());
		mob.accelerate();
		System.out.println(mob.getSpeed());
		mob.accelerate();
		System.out.println(mob.getSpeed());
		mob.accelerate();
		System.out.println(mob.getSpeed());
		mob.accelerate();
		System.out.println(mob.getSpeed());
		mob.brake();
		System.out.println(mob.getSpeed());
		mob.brake();
		System.out.println(mob.getSpeed());
		mob.brake();
		System.out.println(mob.getSpeed());
		mob.brake();
		System.out.println(mob.getSpeed());
		mob.brake();
		System.out.println(mob.getSpeed());
		
	}

	public int getYearModel() {
		return yearModel;
	}

	public void setYearModel(int yearModel) {
		this.yearModel = yearModel;
	}

	public String getMake() {
		return make;
	}

	public void setMake(String make) {
		this.make = make;
	}

	public int getSpeed() {
		return speed;
	}

	public void setSpeed(int speed) {
		this.speed = speed;
	}
	
	public void accelerate(){
		speed += 5;
		
	}
	
	public void brake(){
		speed -= 5;
		if (speed < 0) speed = 0;
	}
	
}
