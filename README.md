## ASP Repositories and Dependency Injection
Simple ASP project to demonstrate the repository pattern and dependency injection.

### Explanation
This is a simple blog program which allows users to create and share posts. To store posts, there is an interface
called `IBlogRepository` which has methods for retrieving and adding posts.  
There are two implementations of this interface: `InMemoryBlogRepository`, which stores data in a list in memory,
and `JsonBlogRepository`, which writes data to a JSON file. To switch between them, simply modify line 5
in `program.cs`:  
<img width="635" height="29" alt="implement-repository" src="https://github.com/user-attachments/assets/ce7775ff-e4a5-4045-b0bd-e900da9ded6f" />  
Switch `JsonBlogRepository` with `InMemoryBlogRepository`

  To access the repository, the pages use Dependency Injection in the constructors:  
  <img width="595" height="138" alt="dependency-injection" src="https://github.com/user-attachments/assets/9c185289-7402-4c26-bdb4-f0e31786d8b9" />

  
