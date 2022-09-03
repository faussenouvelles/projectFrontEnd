# projectFrontEnd

<!DOCTYPE html>
<html>
  <head>
    <meta charset="UTF-8" />
    <title>Template</title>

    <!-- bootstrap css -->
    <link
      rel="stylesheet"
      href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css"
    />

    <!-- don't use this in production: -->
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
  </head>
  <body>
    <!-- we will put our teact component inside this div -->
    <div id="root"></div>

    <!-- load react -->
    <script src="https://unpkg.com/react/umd/react.development.js" crossorigin></script>
    <script src="https://unpkg.com/react-dom/umd/react-dom.development.js" crossorigin></script>
    <script src="https://unpkg.com/react-router@5.2.1/umd/react-router.min.js" crossorigin></script>
    <script src="https://unpkg.com/react-router-dom@5.2.1/umd/react-router-dom.min.js" crossorigin></script>

    <!-- load our react component. -->
    <script src="context.js" defer type="text/babel"></script>
    <script src="navbar.js" defer type="text/babel"></script>
    <script src="createaccount.js" defer type="text/babel"></script>
    <script src="login.js" defer type="text/babel"></script>
    <script src="deposit.js" defer type="text/babel"></script>
    <script src="withdraw.js" defer type="text/babel"></script>
    <script src="balance.js" defer type="text/babel"></script>
    <script src="alldata.js" defer type="text/babel"></script>
    <script src="home.js" defer type="text/babel"></script>
    <script src="index.js" defer type="text/babel"></script>
    <script>
    function Spa() {
  return (
    <HashRouter>
      <NavBar/>
      <UserContext.Provider value={{users:[{name:'abel',email:'abel@mit.edu',password:'secret',balance:100}]}}>
        <div className="container" style={{padding: "20px"}}>
          <Route path="/" exact component={Home} />
          <Route path="/CreateAccount/" component={CreateAccount} />
          <Route path="/login/" component={Login} />
          <Route path="/deposit/" component={Deposit} />
          <Route path="/withdraw/" component={Withdraw} />
          <Route path="/balance/" component={Balance} />
          <Route path="/alldata/" component={AllData} />
        </div>
      </UserContext.Provider>      
    </HashRouter>
  );
}

ReactDOM.render(
  <Spa/>,
  document.getElementById('root')
);
    </script>
  </body>
</html>
