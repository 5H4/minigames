### **Ecommerce game**

<p align="center">
  <img width="300" height="300" src="https://i.ibb.co/LZzwMZ1/spinner.png"/>
</p>

#### **Use point**

##### Logic
* On point use
	* delete point(reward)
* effect -> on target product (these products were no discounted)

#### **Package MiniGames - Spinner**

##### Constructor
* Popup button -> play game
* Open spinner -> spin(random)
	* [15, 25, 35, 45] -> point
	* [100p => 50%] -> discount chance #p is point.
* store point(reward)
* on 100 point -> unlock grab your coupon "JHE5541"

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

<p align="center">
  <img width="353" height="174" src="https://i.ibb.co/r4RwzRw/Screenshot-from-2020-03-31-16-27-18.png"/>
</p>
#### **Package MiniGames - Box**

##### Constructor
* On enter app -> play game
* Open box -> on click box get point 3x
	* max_sum_number = 100 / from array [4, 5, 10, 0]->random
	* exmp: pic from array 4 do { 100 / 4 } = 25 point.
	* array {}
		* { 100 / 4 } = 25 point.
		* { 100 / 5 } = 20 point.
		* { 100 / 10 } = 10 point.
		* { 100 / 0 } = 0 point.
	* BOX_1 + BOX_2 + BOX_3 = POINT
	* store point(reward)


##### INIT Component
* Tree
	* Layout box_ly.xml -> set custom layout.
	* Package MiniGames
		* Box
			* InitBox.class
* Run 
	* InitBox(context)
	
* Return
	* Point (Integer)
		* Logic[ user.point = user.point + (box1 + box2 + box3)]
		* Example: user.point = database(20) + (10, 0, 20) = 50 point










