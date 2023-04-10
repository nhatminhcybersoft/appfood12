# Sequelize appFood
route:
  - Xử lí like nhà hàng
    + POST localhost:4000/api/v1/likeRes/:resId/like    :  // Like/Unlike nhà hàng             
       // Body: { 
        "userId" : "int" 
      }                 
                
    + GET localhost:4000/api/v1/user/:userId              // Lấy danh sách like theo user
    + GET localhost:4000/api/v1/restauranr/:resId         // Lấy danh sách like theo nhà hàng
    
  - Xử lí đánh giá nhà hàng
    + POST localhost:4000/api/v1/rateRes/:resId/rate   :   // Thêm đánh giá              
        // Body: { 
        "userId" : "int",
        "amount" : "int",
        }
       
    + GET localhost:4000/api/v1/rateRes/user/:userId        // Lấy danh sách đánh giá theo user
    + GET localhost:4000/api/v1/rateRes/restaurant/:resId   // Lấy danh sách đánh giá theo nhà hàng
  
  - Order:
    + POST localhost:4000/api/v1/orders/:foodId             : // Thêm order               
        // Body: { 
        "userId" : "int",
        "amount" : "int",
        "code" : "string",
        "arrSubId" : "string"
      }
       
