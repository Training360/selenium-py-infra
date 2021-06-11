# 015 Feladat Conduit - új post
A feladatod, hogy a conduit-app forkodat felkészítsd Github Actions futtatásra és az előzőekben elkészített Selenium IDE projekteket lefuttasd siderunner segítségével.

A `selenium-tests` mappát kell használnia a Github Actions workflow-nak. Ebben vannak az előzőleg beküldött `.side` fájljaid. 

A workflow scripthez az alábbiakat használd:

Nodejs telepítés
```
- name: install Nodejs
  uses: actions/setup-node@v2
  with:
    node-version: '14'
```

Selenium Side Runner telepítése:
```
- name Install Selenium Side Runner
  run: |
    npm install -g selenium-side-runner
```

Chrome böngésző telepítése:
```
- name: Install Chrome
  run: |
    sudo apt install google-chrome-stable
```

Selenium webdriver telepítő program linuxra
```
- name: Install seleniumbase
    run: pip install seleniumbase
```

Chromedriver telepítés
```
- name: Install chromedriver
    run: |
      seleniumbase install chromedriver
```

Side runner futtatása:
Itt ügyeljünk arra, hogy a lent látható paramétereket átadjuk a futtató környezetnek. Nem akarjuk grafikusan megjeleníteni a böngészőt, mert ezeknek a futtató gépeknek nincs grafikus környzete!
```
 - name: Run Tests
        run: |
          selenium-side-runner -c "browserName=chrome goog:chromeOptions.args=[disable-infobars, headless]" test.side
```

Beadni a Github Action workflow-t kell.
