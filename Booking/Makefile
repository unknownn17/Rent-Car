run:
	go run cmd/main.go
table:
	migrate create -dir ./storage/migrations -ext sql db
table-up:
	migrate -path ./storage/migrations -database "postgres://postgres:2005@localhost:5432/rent?sslmode=disable" up
table-down:
	migrate -path ./storage/migrations -database "postgres://postgres:2005@localhost:5432/rent?sslmode=disable" down
table-force:
	migrate -path ./storage/migrations -database "postgres://postgres:2005@localhost:5432/rent?sslmode=disable" force