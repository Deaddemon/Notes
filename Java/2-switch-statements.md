Switch statement

```.java

	case “Saturday”, “Sunday” -> System.out.println(“8AM”);
	//is same as:
	case “Saturday”, “Sunday”:
			System.out.println(“8AM”);
			break;
	//to return a value from switch statement:
        case “Saturday”, “Sunday” -> result = “8AM”;


	result = switch(day){
		case “Saturday”, “Sunday” : yield “6am”;
	};
	//is same as:
	result = switch(day){
		case “Saturday”, “Sunday” ->  “6am”;
	};

```
