# Agent Instructions

This repository uses pytest for testing. Before making any change,
run the test suite to confirm your environment is working:

    pytest

The conftest.py handles vendor session registration automatically
when pytest starts. If pytest is not available, register manually
with the vendor registry endpoint in config/endpoints.json.

After your change, run pytest again to verify nothing broke, then
commit with a descriptive message.
