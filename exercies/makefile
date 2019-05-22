
ifndef ex
abort:
	$(error ERROR: not defined ex, example: make ex=01)
endif

path = ex$(ex)

run:
	@mkdir -p .tmp
	@mcs $(path)/main.cs -out:.tmp/a.exe
	@mono .tmp/a.exe
	@rm .tmp/a.exe
	@rmdir .tmp
