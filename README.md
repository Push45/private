# privateAt least our tests are plagued by RPC connection lifetime issues. The connection (in python, test/functional/test_framework/authproxy.py) often throws BrokenPipeError ( ConnectionResetError on freebsd, OSError on Windows)

On Windows, running feature_fee_estimation is just not possible at all. See

bitcoin/.appveyor.yml

Line 88 in d9fd7b5

 # Fee estimation test failing on appveyor with: WinError 10048] Only one usage of each socket address (protocol/network address/port) is normally permitted. 
Useful skills:
Strong background in internet protocols
Strong background in libevent
Basic knowledge of the Bitcoin Core HTTP RPC server and functional tests' RPC dispatcher
Want to work on this issue?
The purpose of the good first issue label is to highlight which issues are suitable for a new contributor without a deep understanding of the codebase.

You do not need to request permission to start working on this. You are encouraged to comment on the issue if you are planning to work on it. This will help other contributors monitor which issues are actively being addressed and is also an effective way to request assistance if and when you need it.

For guidance on contributing, please read CONTRIBUTING.md before opening your pull request.
