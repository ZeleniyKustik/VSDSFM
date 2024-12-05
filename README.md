# VSDSFM
Very Simple Data Storage For Mindustry

```mermaid
graph TD
    user(User) 
    main(Main)
    core(Cores)

    port[Port]
    mem[Memory]
    memcore[Core memory]



    user --> |query| port
    port --> |ansver| user

   
    main <--> mem
    main <--> memcore
    main <--> port


    core <-->  memcore
core <--> |data| port
    core -->|write| mem
    mem -->|read| core
    
  


```
