Type Narrowing: 
Type narrowing in TypeScript is the process of refining a broader type to a more specific type within a specific path of execution. TS uses control flow analysis to look at your runtime JS code and automatically  infer when a type has been safely restricted.

Practical Examples:

typeof :
It is used to narrow primitive types life string, number, boolean or symbol.

here is the code,

function format(value: string | number) {
  if (typeof value === "string") {
    return value.toUpperCase();
  }
  return value.toFixed(2);
}


instance of : 
This operator is used for checking whether an object is an instance of a specific class or constructor function.

here is the code, 

function printInfo(obj: Date | string) {
  if (obj instanceof Date) {
    return obj.toISOString(); 
  }
  return obj; 
}


in: 
in operator is used to check for the existence of a property on an an object, helping narrow down union types of distinct object shapes.

here is the code, 

type Admin = { privileges: string[] };
type User = { name: string };

function checkAccess(account: Admin | User) {
  if ("privileges" in account) {
    console.log(account.privileges); 
  }
}