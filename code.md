# Code
Below are examples of code I have written: 

## HTML
    <!DOCTYPE html>
    <html>
    <head>
    <meta charset="UTF-8">
    <title>Fizz Buzz</title>
    <script>
    for (var i=1; i < 101; i++){
        if (i % 15 == 0) console.log("FizzBuzz")
        else if (i % 3 == 0) console.log("Fizz");
        else if (i % 5 == 0) console.log("Buzz");
        else console.log(i);
    }
    function fizzbuzz() {
	    var display = document.getElementById    ('display');
	    var displayHTML = "";
	    for (i = 0; i < 100; i++) {
		    displayHTML += "<p>" + i + "</p>";
	    }
	    display.innerHTML = displayHTML
    }

    </script>

    </head>

    <body onload="fizzbuzz()">
    <div id="display">

    </div>
    </body>

    </html>

## Python
def main():

    import math
    while (True):
        try:
                r=float(input("Radius of Cylinder:"))
                if(r < 0):
                    print("Negative numbers not allowed, try number greater than 0.")
                    continue
        except ValueError:
                    print("Error: Enter a positive number.")
        else:
                    break
    while (True):
        try:
                h=float(input("Height of Cyclinder:"))
                if(h < 0):
                    print("Negative numbers not allowed, try number greater than 0.")
                    continue
        except ValueError:
                    print("Error: Enter a positive number.")
        else:
                    break
    volume=math.pi*pow(r,2)*h

    print("Volume of Cyclinder: %.2f" %volume)

    restart=input("Do you want to find another volume, 'yes' or 'no'.").lower()
    if restart == "yes":
        main()
    else:
        exit()
    main()

 [Home Page](./README.md)