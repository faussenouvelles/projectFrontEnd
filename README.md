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
    <script>
    <nav className="navbar navbar-expand-lg navbar-light bg-light">
      <a className="navbar-brand" href="#">BadBank</a>
      <button className="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span className="navbar-toggler-icon"></span>
      </button>
      <div className="collapse navbar-collapse" id="navbarNav">
        <ul className="navbar-nav">
          <li className="nav-item">
            <a className="nav-link" href="#/CreateAccount/">Create Account</a>
          </li>
          <li className="nav-item">
            <a className="nav-link" href="#/login/">Login</a>
          </li>
          <li className="nav-item">
            <a className="nav-link" href="#/deposit/">Deposit</a>
          </li>
          <li className="nav-item">
            <a className="nav-link" href="#/withdraw/">Withdraw</a>
          </li>
          <li className="nav-item">
            <a className="nav-link" href="#/balance/">Balance</a>
          </li>
          <li className="nav-item">
            <a className="nav-link" href="#/alldata/">AllData</a>
          </li>          
        </ul>
      </div>
    </nav>
    </>
</script>
    <script src="createaccount.js" defer type="text/babel"></script>
    <script src="login.js" defer type="text/babel"></script>
    <script src="deposit.js" defer type="text/babel"></script>
    <script src="withdraw.js" defer type="text/babel"></script>
    <script src="balance.js" defer type="text/babel"></script>
    <script src="alldata.js" defer type="text/babel"></script>
    <script src="home.js" defer type="text/babel"></script>
    <script src="index.js" defer type="text/babel"></script>
  </body>
</html>
