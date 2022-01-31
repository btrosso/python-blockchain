**Setup the virtual environment**
```
python -m venv blockchain-env
```

**Activate the virtual environment**
```
C:\Users\btros\python-blockchain\blockchain-env\Scripts\activate.bat
```

**Install all packages**
```
pip3 install -r requirements.txt
```

**Run the tests**

Make sure to activate the virtual environment.

```
python -m pytest backend/tests
```

**Run the application and API**
```
python -m backend.app
```

**Run a peer instance**
Make sure to use Git Bash, by clicking inside the project folder and running the CLI from there.
Make sure to activate the virtual environment.

```
export PEER=True && python -m backend.app
```

**Run the frontend**

In the frontend directory:
```
npm run start
```

**Seed the backend with data**
Make sure to activate the virtual environment.
```
export SEED_DATA=True && python -m backend.app
```


***Demonstration steps:***
Demo 1 Notes: General
1. open file explorer here: C:\Users\btros\source\repos\python-blockchain
2. right click > GIT BASH here (window A)
3. run these commands on window A:
	a. source blockchain-env/Scripts/activate
	b. export SEED_DATA=True && python -m backend.app
4. open file explorer here: C:\Users\btros\source\repos\python-blockchain
5. right click > GIT BASH here (window B)
6. run these commands on window B:
	a. source blockchain-env/Scripts/activate
	b. export PEER=True && python -m backend.app
7. open file explorer here: C:\Users\btros\source\repos\python-blockchain\frontend
8. right click > GIT BASH here (window C)
9. run these commands on window C:
	a. npm run start
-------------------------------------------------------------------
Demo 2 Notes: to demonstrate mining and adding new blocks:
1. open file explorer here: C:\Users\btros\source\repos\python-blockchain
2. right click > GIT BASH here (window A)
3. run these commands on window A:
	a. source blockchain-env/Scripts/activate
	b. python -m backend.app
4. open file explorer here: C:\Users\btros\source\repos\python-blockchain
5. right click > GIT BASH here (window B)
6. run these commands on window B:
	a. source blockchain-env/Scripts/activate
	b. export PEER=True && python -m backend.app
7. open file explorer here: C:\Users\btros\source\repos\python-blockchain\frontend
8. right click > GIT BASH here (window C)
9. run these commands on window C:
	a. npm run start	
10. open new tab in google: http://localhost:5000/blockchain/mine
	-- keep refreshing to watch command windows update
	-- to demonstrate another user mining switch the 5000 in the above url to whatever 
		the other local host IP address is in the PEER instance and refresh