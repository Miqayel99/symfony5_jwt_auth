Here are routes for  API &#8595;

register:
  path: /register
  controller: App\Controller\AuthController::register
  methods: [ POST ]

api:
  path: /api
  controller: App\Controller\AuthController::api

create:
  path: /user/create
  controller: App\Controller\UserController::create
  methods: [POST]

delete:
  path: /user/delete
  controller: App\Controller\UserController::delete
  methods: [ POST ]

edit:
  path: /user/edit
  controller: App\Controller\UserController::edit
  methods: [ POST ]

view:
  path: /user/view/{email}
  controller: App\Controller\UserController::view
  methods: [ GET ]

app:
  path: /{params}
  controller: App\Controller\DefaultController::index
  requirements:
    params: "^(?!admin|api).+"

api_login_check:
  path: /api/login_check
  controller: App\Controller\AuthController::login
  methods: [ POST ]
  And here are Postman request examples &#8595;
  ![1forRegister](https://user-images.githubusercontent.com/81144308/117012817-5bff5f00-ad00-11eb-9de0-5dd4bac0fb7c.png)
![2forLogin](https://user-images.githubusercontent.com/81144308/117012820-5d308c00-ad00-11eb-8f7e-0d271b7ed56e.png)
![3 2forCreate](https://user-images.githubusercontent.com/81144308/117012824-5d308c00-ad00-11eb-84e8-1ec04bb347df.png)
![3forCreate](https://user-images.githubusercontent.com/81144308/117012825-5dc92280-ad00-11eb-98c3-3b1f6630fcc7.png)
![4forDelete](https://user-images.githubusercontent.com/81144308/117012829-5dc92280-ad00-11eb-9fff-b52f8644c340.png)
![5forEdite](https://user-images.githubusercontent.com/81144308/117012831-5e61b900-ad00-11eb-8a50-5b3dc9c13317.png)
![6forView](https://user-images.githubusercontent.com/81144308/117012832-5e61b900-ad00-11eb-8551-50c35cf7ba95.png)

