# clothe-billing-

public class ProductDiscountCalculator {
    double price,amount,finalamount;
  String  disc;
    String name,product;
    int qty;
    boolean exe;
    public void customerDetail(){
        System.out.println("customer name : "+name);
        System.out.println("product name : "+product);
        System.out.println("product  price : "+price);
        System.out.println("product qty : "+qty);
        

    }  
    public void totalAmt(){
         amount=price*qty;
         System.out.println("total amount : "+amount);
         System.out.println("discount on the product : "+disc);
         if(exe==true){
         finalamount=amount*30/100;
         finalamount=amount-finalamount;
         System.out.println("total payable amount : "+finalamount);
         }
         System.out.println();
         System.out.println();
         
          if(exe==false)  {
            finalamount=amount*20/100;
         finalamount=amount-finalamount;
         System.out.println("total payable amount : "+finalamount);
         }
         
    } 
    public static void main(String[] args){
        ProductDiscountCalculator p1= new  ProductDiscountCalculator();
        p1.price=1500;
        p1.name="sagar sahu";
        p1.product="jeans";
        p1.qty=2;
        p1.disc="30%";
        p1.exe=true;  
        p1.customerDetail();
        p1.totalAmt();
        ProductDiscountCalculator p2= new  ProductDiscountCalculator();
        p2.price=300;
        p2.name="sagar sahu";
        p2.product="unbranded  tshirt";
        p2.qty=2;
        p2.disc="20%";
        p2.exe=false;
        
        p2.customerDetail();
        p2.totalAmt();
    } 
    
}
