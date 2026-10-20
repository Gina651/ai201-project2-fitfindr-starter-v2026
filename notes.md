# Milestone 1: Data Exploration

## What I Learned

I explored six clothing listings and examined the fields available in the dataset. Some important fields include `title`, `description`, `category`, `style_tags`, `size`, `price`, `condition`, `colors`, `brand`, and `platform`.

One thing I noticed is that clothing sizes are not always consistent. The six listings use different size formats, including W30 L30, S/M, XL (oversized), M, W28, and L. For example, the Y2K Baby Tee is listed as S/M, but its description says it fits more like a small. This means my search tool needs to consider different size formats instead of relying only on exact matches.

For the query "vintage graphic tee under $30, size M," listing `lst_002` is a possible match because it costs $18, has the graphic tee and vintage style tags, and is labeled S/M. However, an exact size comparison would miss it. I will need to decide how to handle sizes like S/M when defining my acceptance criteria.

I also noticed that style tags can help identify items that match a user's preferences, even when the exact words are not in the title.

Another observation is that some listings have no brand information. For example, `lst_002`, `lst_005`, and `lst_006` have `null` as their brand. My search tool should handle missing brand values without crashing.

## Starter Test

I successfully ran the starter application using the query `vintage graphic tee under $30`.

The application displayed the expected message that the planning loop has not been built yet. This confirms that the starter runs correctly before implementing the tools and agent.

## Next Steps

My next step is to define the three required tools, write measurable acceptance criteria, and build the planning loop that connects the tools together.