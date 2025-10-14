# Agentforce Vibes IDE Release Notes

Each release typically contains bug fixes, as well as performance and security enhancements. We recommend that you upgrade to the latest version to enhance security and performance.

These release notes outline the changes of note in the latest Agentforce Vibes IDE release.

## Oct 13 2025

**More Information About Agentforce Vibes Access from Setup Menu**

Currently, Agentforce Vibes appears under the Setup gear menu for all users. To access Agentforce Vibes, users must have the `View All Data` permission. Those without this permission will see an error message prompting them to contact their administrator for access.
Developers can access Agentforce Vibes from Sandboxes without requiring production access, where they typically have higher-level permissions.

## Oct 10th 2025

Formerly known as Agentforce Vibes IDE, the Agentforce Vibes IDE is now accessible directly from your Salesforce org! This modern, web-based IDE delivers the full power of Visual Studio Code in your browser, complete with Salesforce Extensions, the Salesforce CLI, and GitHub integration.
Launch from your org’s Setup menu to get an instantly authenticated, org-aware environment where your metadata automatically loads into an SFDX project—no manual setup required.


## August 28th 2025

We’ve updated the org authentication flow to align with [Salesforce CLI changes](https://github.com/forcedotcom/cli/issues/3368). The Connected App authorization flow now uses Web Auth and delivers a more reliable authentication experience.

As a result of this change, a very small subset of our users might see an `Invalid Authentication State` error during active transition to Web Auth. We recommend that you don't use the Agentforce Vibes IDE instance during this transition. If you encounter this error, the wait time for an instance to refresh is around 15 minutes. We apologize in advance for any inconvenience this may cause. 

Some users might see an `{"error":"Unable to complete authorization."}` error.  If you encounter this error, reset your environment and try again. Create an [issue](https://github.com/forcedotcom/code-builder-feedback/issues) if the error persists.

## Jul 15 2025

- :tada: :rocket: We’re excited to announce that Agentforce Vibes IDE is now accessible in sandbox environments. Once an admin has accepted the Agentforce Vibes IDE Terms and Conditions and assigned the necessary permissions, users can launch Agentforce Vibes IDE directly from sandboxes.
This enhancement streamlines development workflows by enabling seamless access to Agentforce Vibes IDE in non-production orgs - bridging the gap between sandbox and production environments and equipping developers with powerful, consistent tooling throughout the development lifecycle.
Get Ready! We’re rolling out this feature in waves—starting with 10% of orgs and expanding by an additional 20% each week until everyone has access. Keep an eye out—it’s coming your way soon!

## v1.3.0 (Sep 25, 2024) 

- We made a significant improvement in the startup time for Agentforce Vibes IDE instances. The version number is still 1.3.0 because this is an infrastructure change rather than an update to the Agentforce Vibes IDE package.

## v1.3.0 (May 3, 2024) 

- Removed the Environments tab, which represents object metadata. This change eliminates unnecessary user interaction with the object, reducing the risk of unintended changes that could break the environment.
