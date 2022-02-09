Runtime Releases
These checks should be performed on the codebase.

 Verify spec_version has been incremented since the last release for any native runtimes from any existing use on public (non-private/test) networks.
 Verify previously completed migrations are removed for any public (non-private/test) networks.
No migrations added in the last release that would need to be removed.
 Verify pallet and extrinsic ordering as well as SignedExtensions have stayed the same. Bump transaction_version if not.
 Verify new extrinsics have been correctly whitelisted/blacklisted for proxy filters.
No new extrinsics.
 Verify benchmarks have been updated for any modified runtime logic.
 Verify the weights are up-to-date.
 Verify that the various pieces of XCM config are sane.
The following checks can be performed after we have forked off to the release- candidate branch or started an additional release candidate branch (rc-2, rc-3, etc)

 Verify new migrations complete successfully, and the runtime state is correctly updated for any public (non-private/test) networks.
 Run integration tests.
 Teleport Relay -> Statemin* and back.
 Create asset (if applicable), mint and transfer
 Push runtime upgrade to Westmint and verify network stability.
