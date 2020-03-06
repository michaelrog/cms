# Running Release Notes for Craft CMS 3.5

### Added
- Added the “Use shapes to represent statuses” user preference. ([#3293](https://github.com/craftcms/cms/issues/3293))
- It’s now possible to set a custom route that handles Set Password requests. ([#5722](https://github.com/craftcms/cms/issues/5722))
- Added the `drafts`, `draftOf`, `draftId`, `draftCreator`, `revisions`, `revisionOf`, `revisionId` and `revisionCreator` arguments to element queries using GraphQL API. ([#5580](https://github.com/craftcms/cms/issues/5580)) 
- Added the `isDraft`, `isRevision`, `sourceId`, `sourceUid`, and `isUnsavedDraft` fields to elements when using GraphPQL API. ([#5580](https://github.com/craftcms/cms/issues/5580))
- Added the `assetCount`, `categoryCount`, `entryCount`, `tagCount`, and `userCount` queries for fetching the element counts to the GraphPQL API. ([#4847](https://github.com/craftcms/cms/issues/4847))
- Added the `locale` argument to the `formatDateTime` GraphQL directive. ([#5593](https://github.com/craftcms/cms/issues/5593))
- Added `craft\web\AssetBundle\ContentWindowAsset`.
- Added `craft\web\AssetBundle\IframeResizerAsset`.
- Added the [iFrame Resizer](http://davidjbradshaw.github.io/iframe-resizer/) library.

### Changed
- Preview frames now maintain their scroll position across refreshes, even for cross-origin preview targets.
- Preview targets that aren’t directly rendered by Craft must now include `lib/iframe-resizer-cw/iframeResizer.contentWindow.js` in order to maintain scroll position across refreshes.
- The preview frame header no longer hides the top 54px of the preview frame when it’s scrolled all the way to the top. ([#5547](https://github.com/craftcms/cms/issues/5547))
- The `QueryArgument` GraphQL type now also allows boolean values.