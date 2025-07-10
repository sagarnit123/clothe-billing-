# clothe-billing-

// Source code is decompiled from a .class file using FernFlower decompiler.
public class ProductDiscountCalculator {
   double price;
   double amount;
   double finalamount;
   String disc;
   String name;
   String product;
   int qty;
   boolean exe;

   public ProductDiscountCalculator() {
   }

   public void customerDetail() {
      System.out.println("customer name : " + this.name);
      System.out.println("product name : " + this.product);
      System.out.println("product  price : " + this.price);
      System.out.println("product qty : " + this.qty);
   }

   public void totalAmt() {
      this.amount = this.price * (double)this.qty;
      System.out.println("total amount : " + this.amount);
      System.out.println("discount on the product : " + this.disc);
      if (this.exe = true) {
         this.finalamount = this.amount * 30.0 / 100.0;
         this.finalamount = this.amount - this.finalamount;
         System.out.println("total payable amount : " + this.finalamount);
      }

      System.out.println();
      System.out.println();
      if (this.exe = false) {
         this.finalamount = this.amount * 20.0 / 100.0;
         this.finalamount = this.amount - this.finalamount;
         System.out.println("total payable amount : " + this.finalamount);
      }

   }

   public static void main(String[] var0) {
      ProductDiscountCalculator var1 = new ProductDiscountCalculator();
      var1.price = 1500.0;
      var1.name = "sagar sahu";
      var1.product = "jeans";
      var1.qty = 2;
      var1.disc = "30%";
      var1.exe = true;
      var1.customerDetail();
      var1.totalAmt();
      ProductDiscountCalculator var2 = new ProductDiscountCalculator();
      var2.price = 300.0;
      var2.name = "sagar sahu";
      var2.product = "unbranded  tshirt";
      var2.qty = 2;
      var2.disc = "20%";
      var2.exe = false;
      var2.customerDetail();
      var2.totalAmt();
   }
}
