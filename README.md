##CPU, Memory profiling
- go test ./... -cpuprofile cpu.prof -count 100000
- go tool pprof -web <package>.test.exe cpu.prof
- go tool pprof <package>.test.exe cpu.prof, help, top10, list <pattern match>, weblist <pattern match>
- go test ./... -memprofile mem.prof -count 100000
- go pprof -web <package>.test.exe mem.prof
- go pprof <package>.test.exe mem.prof, help, top 5, list <pattern>
- go tool pprof http://localhost:3000/debug/pprof/profile
- go tool pprof http://localhost:3000/debug/pprof/heap
- go tool pprof http://localhost:3000/debug/pprof/block