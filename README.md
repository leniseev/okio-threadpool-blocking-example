# Tokio threadpool blocking demo

In this demo Tokio thread_pool blocking feature is presented.

8 "heavy computation" blocking features are spawned, after which 8 non-blocing features are spawned too.
Each blocking feature enters blocking environment and performs heavy computation for 1 second.

One can see that non-blocking features return before blocking ones, despite being started later.

## Running
`cargo run`