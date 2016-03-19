## Security
### Passport

    app.post('/login',
      passport.authenticate('local', { successRedirect: '/',
                                   failureRedirect: '/login'});
                                   );
