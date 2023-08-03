# Next-js

Rendering
React render it on client side
Next can do both on option
Client side rendering => when u send request to server he send you html and js file then it renders on client side on browser
Server side rendering => it render them in server then shows you in browser immediately

SEO
Next send pre-rendered code directly to the client this lead easy Easy crawling and Indexing by search engines, leading to improve SEO

Advantages of SEO  
-Increased organic traffic
-Enhanced user experience
-Credibility and trustworthiness
-Competetive advantage

Routing
React => react router dom
Next => file system 

If there is react hooks useState,useEffect it should be slient side rendering, add on top ‘use client’ otherwise it will show error.
Next js documentation suggest to you when to use server or client side	

Data Fetching 
1. Server Side Rendering (SSR) cache:no
2. Static Side Generation (SSG) default 
3. Incremental Static Generation(ISG)

We can define Metadata in two ways: Static and Dynamic
1 Static Metada 
export const metadata = {
  title:"Home",
}
Output => <head> <title>My unique product"</title></head>
2 Dynamic Metada 
export async function generateMetaData({params,searchParams}){
  const product = await getProduct(params.id);
  return { title:product.title }
  Output => <head> <title>My unique product"</title></head>




















  
