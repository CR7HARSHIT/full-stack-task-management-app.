" FoodDeliveryApplication" 
My app routing is handled using React Router, and it follows this structure:

Main Layout (AppLayout)

Wraps the entire app with Redux (Provider) and UserLocationContext.
Contains common components: Header, Outlet (for pages), and Footer.
Routes Setup (appRouter)

"/" → Home Page (Body component).
"/about" → About Us Page.
"/contact" → Contact Page.
"/city/:rest-name-id" → Dynamic Route for Restaurant Menu (changes based on rest-name-id).
"/cart" → Cart Page.
Each route is a child of AppLayout, so they all share the same Header and Footer while the Outlet displays the page based on the route.

*****
All the components code is present in Component folder.
I Have use Redux Store(Large Scale Application) for global state management
 Store setup code-App folder
 cart Slice Code-features folder
I have also used Custom Hooks
code files-utils


*******
Project flow(Can Also See Developer Console )()
1. when we open the Application(It Will ask longitude and latitude cordinates based on that )
2.It will provide an list of resaturent menu cards providing online food delivery services near that Location.
3. I am basically using swiggy api to fetch restaurent data(Not free got from Network in developer console to
show that i can handle real data and can manipulate it effectively )
4.On hitting  any restaurent card you will get redirected to restaurent menu page.
5. I have build accodian features where if an accodian is already open if we try to open another one the 
previous one will shut down. 
6.For cart functionality i have used Redux Store and created an cart slice for it.
7.You can add items and delete items from  resaturent menu page  it will reflect in cart  and viceversa.
8. Built an Online Offline feature. 
