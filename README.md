👋 Hi there! I'm Martin-Louis Bright, a software engineer living in Toronto, Canada, with over [20 years of experience][cv] in information technology.

I'm a networking generalist: overlays and encapsulation, default-deny access, IPv6 addressing, and working out what encrypted traffic is up to without reading it.
If it has a header, I want to know what's in it.
I enthusiastically use Wireshark, SSH, and Tailscale.

Code is cheap now.
Agents write most of my Python, Go, Rust, C, Bash, and Terraform, usually from a few tmux panes at once.
I read every line, but I don't pick projects by language anymore.
What's scarce is understanding: which bytes are on the wire, what the kernel actually does with them, and whether the thing works or merely compiles.

My career-long pledge to avoid languages prefixed with 'Java' is now enforced by my agents.

**Things I've built lately:**

- [decapsulator][decapsulator]: an XDP program that strips up to three nested layers of VXLAN/GENEVE at the driver.
- [maxvxlanthroughput][maxvxlanthroughput]: tuning for hosts that terminate VXLAN/Geneve tunnels, plus a kernel-source check showing the popular UDP-throughput settings don't help VXLAN.
- [xdpgate][xdpgate]: an XDP default-deny gate that drops packets unless an fwknop Single Packet Authorization has opened the exact flow.
- [confetti][confetti]: fwknop opens short-lived EC2 security group holes, and a timer closes them.
- [ipv6rd][ipv6rd]: watches netlink and re-knocks when your IPv6 privacy address rotates, so you don't lock yourself out.
- [ushape][ushape]: classifies encrypted traffic from packet sizes and timing, never the payload.

I'm currently working at [cPacket Networks][cpacket], where I operate mainly in [AWS][aws] and [Azure][azure].
Before that, I was a [GitHub Enterprise][ghes] [site administrator][github-site-admin] at [Autodesk][autodesk].
I'm at home on Linux ([Ubuntu][ubuntu], still) and macOS, I think infrastructure as code and [GitOps][gitops] are great, and I embraced [devops culture][devops] before it had a name.

An archived repository in this space means that it has few or no end users, or that it is an experiment that has run its course.
The archived repos here are unmaintained, however if you have questions about them, feel free to reach out via old-fashioned email.

[cv]: https://mlbright.github.io/cv/
[decapsulator]: https://github.com/mlbright/decapsulator
[maxvxlanthroughput]: https://github.com/mlbright/maxvxlanthroughput
[xdpgate]: https://github.com/mlbright/xdpgate
[confetti]: https://github.com/mlbright/confetti
[ipv6rd]: https://github.com/mlbright/ipv6rd
[ushape]: https://github.com/mlbright/ushape
[cpacket]: https://www.cpacket.com/
[aws]: https://aws.amazon.com/
[azure]: https://portal.azure.com
[ghes]: https://github.com/enterprise
[github-site-admin]: https://github.com/mlbright/github-enterprise-site-admin
[autodesk]: https://www.autodesk.com/
[ubuntu]: https://ubuntu.com/
[gitops]: https://www.gitops.tech/
[devops]: https://en.wikipedia.org/wiki/DevOps
