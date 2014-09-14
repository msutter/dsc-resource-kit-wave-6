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

Composite Resource: xIisWordPressSite
- Add xIisWordPressSite.schema.mof file as an example how to include a composite resource in the build of the puppet types.

## Notes

Be aware that the composite resources in this resource kit are not automaticaly discovered from the puppet dsc module at types build time.
If you'd like to generate a puppet type for them, you have to manually create a xxx.schema.mof file next to the xxx.schema.psm1 file.

Look at the xWordPress/DscResources/xIisWordPressSite/xIisWordPressSite.schema.mof as an example.


