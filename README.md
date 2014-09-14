## DSC Resource Kit Wave 6

This Repo is a fixed version of the [DSC Resource Kit Wave 6](http://gallery.technet.microsoft.com/scriptcenter/DSC-Resource-Kit-All-c449312d)

The fixes are for compatibility with the [puppet dsc module](https://github.com/msutter/puppet-dsc)

## Fixes

Resource: xRemoteDesktopAdmin
- renaming class xRemoteDesktopAdmin to MSFT_xRemoteDesktopAdmin

Resource: MSFT_xWindowsOptionalFeature
- Change validateset of ensure from 'enable,disable' to 'present,absent' and adapt the ps code

Resource: MSFT_xWordPressSite
- Add Absent to valuemap in mof schema


