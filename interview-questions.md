# Cloud Network Engineer — Interview Q&A

## Q1: VPC kya hota hai?
VPC (Virtual Private Cloud) ek isolated network hai AWS cloud mein jahan 
hum apne resources deploy karte hain. Jaise ek private office network.

## Q2: Public aur Private subnet mein difference?
- Public Subnet: Internet Gateway se connected, internet se directly accessible
- Private Subnet: Internet se directly accessible nahi, sirf NAT Gateway se outbound traffic

## Q3: Security Group aur NACL mein difference?
- Security Group: Instance level firewall, stateful
- NACL: Subnet level firewall, stateless

## Q4: NAT Gateway kyun use karte hain?
Private subnet ke servers ko internet se updates lene deta hai
lekin internet se directly access nahi hone deta. Security ke liye.

## Q5: Internet Gateway kya karta hai?
VPC aur internet ke beech bridge ka kaam karta hai.
Public subnet ka traffic IGW se bahar jaata hai.

## Q6: Route Table kya hota hai?
Network traffic kahan jaayega yeh define karta hai.
Public subnet ka route IGW ko point karta hai.

## Q7: Subnetting kya hoti hai?
Ek bade network ko chhote parts mein divide karna.
10.0.0.0/16 mein 65,536 IP addresses hote hain.
