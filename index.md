# Steven Christensen
## Software Engineer, Comp Sci Student at UCSD

<img src="IMG_2598.jpg" alt="this is an image" width="200"/>
### Experience

SDE 1 Intern for the Amazon Luna Game Streaming Team


> “I must not fear. Fear is the mind-killer.”

― Frank Herbert, Dune

#### Here is some code that demonstrates adding two numbers represented by linkedlists using recursion
```java
public void sumTwo(LinkedLists l1, LinkedLists l2)
	{
		LinkedLists sumList = new LinkedLists();
		Node n1 = l1.head;
		Node n2 = l2.head;
		
		sumList = sumList.sum(n1, n2, 0, sumList);
		sumList.printList();
	}
	
	public LinkedLists sum(Node n1, Node n2, int carry, LinkedLists sumList)
	{
		int num1, num2, result;
		if(n1 == null && n2 == null) return sumList;
		
		if(n1 != null) num1 = n1.getData();
		else num1 = 0;
		
		if(n2 != null) num2 = n2.getData();
		else num2 = 0;
		
		int sum = num1 + num2 + carry;
		
		if(sum >= 10)
		{
			result = sum - 10;
			carry = 1;
		}
		else
		{
			result = sum;
			carry = 0;
		}
		
		n1 = n1.getNextNode();
		n2 = n2.getNextNode();
		
		this.insert(result);
		
		sumList = this.sum(n1, n2, carry, sumList);
		
		return sumList;
		 
		
	}
```

**Here is a where I have learned everything I know in life**

[Youtube](https://www.youtube.com)

[link](#experience)

[relative-link](README.md)

## Hobbies
- Learning Chinese
- Reading Philosophy
- Working out

## Favorite Animals
1. Ravens
2. Crows
3. Doggos
   
## Task List
  - [ ] update resume
  - [ ] Apply to lots of companies for internships
  - [x] Study a lot

