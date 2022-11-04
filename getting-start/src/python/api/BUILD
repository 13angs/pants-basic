# The default `sources` field will include `main.py`.
python_sources(name="lib")

# Pants will convert the entry point to `helloworld.main`.
pex_binary(
  name="app",
  entry_point="app.py",
)