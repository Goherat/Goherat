import { log } from "console";

let _name : string = `Goher Ali, ABID`;     // Code foe String Type Veriable
log(_name)                      // concole last code

_name=_name.toLowerCase()       // To covert the string in lower case letters
console.log(_name);             // concole to print lower case code

_name=_name.toUpperCase();      // To covert the string in Upper case letters
log(`concole to print Upper case code"`,_name,`"`); // concole to print Upper case code

_name = `Shoukat Ali`       //Over Ride Variable _name
log(_name)

let age :number|string;     //union type variable
age = 12;
age = `45`;
log(age)

let set_of_number : number []= [        // Array of Number only
    1,2,3,4,5,6
]
log("The Array of numbers is", set_of_number)

let set_of_names : string []= [     // Array of String only
    "Muhammad","ahmad","Ali", "Waqas","naveed"
]
log("The set of names",set_of_names)
log(set_of_names.length-1)

let mixed_array : any []=[ //Array includes numbers, string, Boolean
    1,`Usman`,true
 ]
log(mixed_array)

set_of_names.push(`Bakar`);      // Addition of Element "Baker " in string Array at last in number of Array by push metthod
log("After Addition of name by push mehtod 'Bakar':",set_of_names)

log(set_of_names.length-1)      // Code to find the Length of elements in Array

let index_of_set_of_Ali =set_of_names.indexOf(`Ali`)           // HOw to find element named `Ali` in Array
log(index_of_set_of_Ali)                            

let _2nd_element_in_Set_of_names= set_of_names[2];              // How to find what is the element in 3rd number in Array
log(_2nd_element_in_Set_of_names)

set_of_names.pop()      // Code to delete the last element in Array

let deleted_element_by_pop = set_of_names.pop();        // variable to get the name of deleted last element in Array
log("The deleted element by pop is ",deleted_element_by_pop)        //name of last deleted element is Array
log(set_of_names.length)

let deleted_element_by_shift=set_of_names.shift();      // to delete the 1st element is array by useing  shift method
log(deleted_element_by_shift)                   // The name of deleted elemant deleted by shift method
log(set_of_names)

log(set_of_names.length-1)

set_of_names.unshift("Hamddan");        // Addition of Element "Hamddan" in string Array at first in number of Array by unshift metthod

log("The name of 1st elements after addition of element by unshift method", set_of_names);      //Confirmation of Array after Addition of 1st element 
log(set_of_names.length-1)

log(set_of_names);
let _1st_element_by_splice_method=set_of_names.splice(0,1)        // Delete by splice method the 1st and only one element (like shift method)
log(_1st_element_by_splice_method);         // Name of element deleted by splice method
log("console after deletion of 1st element in Array by splice method : ",set_of_names);

let _3st_element_by_splice_method=set_of_names.splice(2,1)      // Delete by splice method the particule selected element "In code 2 disclose the index and 1 disclose that delete 1 element 
log(_3st_element_by_splice_method);
log("console after deletion of 3rd element in Array by splice method : ",set_of_names);

let _Addtion_of_element_by_splice_method=set_of_names.splice(2,0,"Abban","Usman")       // Addition of Element "Abban" & "Usman" in string Array after 2nd Element in number of Array by splice metthod
log(_Addtion_of_element_by_splice_method);
log("console after Addition of 2 new element in Array by splice method : ",set_of_names);

let _replace_2nd_element_in_Array = set_of_names.splice(1,1,"GOher Ali")        //Replacement/Up Gradation of Element "Goher Ali " in place of "ALI" in string Array at 2nd Element in number of Array by splice metthod
log("replaceemt/upgradation of 2nd element in array ", _replace_2nd_element_in_Array)
log(set_of_names);
log(set_of_names.length-1)
set_of_names.splice(4,0,"Muhammad", "Aisha", "Ali", "Fatima", "Omar", "Khadija", "Ahmed", "Sofia", "Zayd", "Layla") // after finding of length we insert 10 more elements in place of 5th and on word
log(set_of_names);
log(set_of_names.length-1)

let copy_of_Array_with_slice=set_of_names.slice(4,9);       //copy Array with slice method from 5th to 9th element and save it an variable for further use.
log("The name of elements copies with slice:",copy_of_Array_with_slice);        // name of copied elements
log(set_of_names)

log(copy_of_Array_with_slice.length-1)

copy_of_Array_with_slice.splice(0,0, "Goher Ali")       // use copied variable and add name with splice method at 1 in Array
log(copy_of_Array_with_slice)
log(copy_of_Array_with_slice.length-1)

function Circle(Dia:number){        //calculate the diameter of circule with function 
    return  + 22/7 * Dia

}
let result= Circle(1)       // Store calculation of Circle in variable named result which is calculated with help of fuction
console.log(result);

const Circle_1 = (Dia:number)=>{     // Store calculation of Circle_1 in variable named result_2 which is calculated with help of "=>"
    return (22/7)*Dia
}
let result_1 :number= Circle_1(2)
console.log(result_1);
let Sub:number=result_1-result  // use that both variables named result_1 & result in an other variable named Sub"
console.log(Sub);

const SuM :any = (num1:number,num2:number,num3?:number):number=>{       // in this code num1 & num2 are mandatory and num3 is optional Or = 0, addition through => function
return num1+num2+(num3||0)
}
console.log(SuM(10,20,30));

