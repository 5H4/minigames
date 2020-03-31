### **Ecommerce game**

<p align="center">
  <img width="300" height="300" src="https://i.ibb.co/LZzwMZ1/spinner.png"/>
</p>

#### **Package MiniGames - Spinner**

##### Constructor
* Popup button -> play game
* Open spinner -> spin(random)
	* [15, 25, 35, 45] -> point
	* [100p => 50%] -> discount chance #p is point.
* store point(reward)
* on 100 point -> unlock grab your coupon "JHE5541"
* delete point(reward)
* effect -> on target product (these products were no discounted)

##### INIT Component
* Tree
	* Layout spinner_ly.xml -> set custom layout.
	* Package MiniGames
		* Spinner
			* InitSpinner.class
* Run 
	* InitSpinner(context)
	
* Return
	* Point (Integer)
		* Logic[ user.point = user.point + GetPoint(getNumber) ]
		* Example: user.point = database(45) + reward(35) = 80 point.









