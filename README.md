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
  
