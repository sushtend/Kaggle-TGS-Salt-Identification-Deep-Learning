# Kaggle TGS Salt Identification Challeneg Using Deep Learning

Several areas of Earth with large accumulations of oil and gas also have huge deposits of salt below the surface.

But unfortunately, knowing where large salt deposits are precisely is very difficult. Professional seismic imaging still requires expert human interpretation of salt bodies. This leads to very subjective, highly variable renderings. More alarmingly, it leads to potentially dangerous situations for oil and gas company drillers.

To create the most accurate seismic images and 3D renderings, TGS (the world’s leading geoscience data company) is hoping Kaggle’s machine learning community will be able to build an algorithm that automatically and accurately identifies if a subsurface target is salt or not.

Seismic data is a neat thing. You can imagine it like an ultra-sound of the subsurface. However, in an ultra-sound, we use much smaller wavelengths to image our body. Seismic data usually has wavelengths around 1m to 100m. That has some physical implications, but for now, we don't have to deal with that. It's just something to keep in mind while thinking about resolution.

Imaging salt has been a huge topic in the seismic industry, basically since they imaged salt the first time. The Society of Exploration geophysicist alone has over 10,000 publications with the keyword salt. Salt bodies are important for the hydrocarbon industry, as they usually form nice oil traps. So there's a clear motivation to delineate salt bodies in the subsurface. If you would like to do a deep dive, you can see this publication

Seismic data interpreters are used to interpreting on 2D or 3D images that have been heavily processed. The standard work of seismic data analysis is open access. You'll find sections on Salt in there as well (https://wiki.seg.org/wiki/Salt-flank_reflections and https://wiki.seg.org/wiki/Salt_flanks). The seismic itself is pretty "old" in the publication, and you're dealing with data that is less noisy here, which is nice.

<b>A little more historical context and some clarifications…</b> by <a href="https://www.kaggle.com/ophiolite">Stef Bernosky</a>

In early days of exploration, it was believed that salt was to be avoided at all costs. It was difficult to image below and provided unacceptable drilling risks. As reservoirs above salt became more exploited and developed, exploration geoscientists had to start exploring the possibilities of sub-salt reservoirs.

Today, sub-salt reservoirs have become less risky to drill and provide the best up-side potential for major oil and gas companies in the United States. Most exploration projects in the Gulf of Mexico today are now sub-salt plays.

Above, it was mentioned that salt is a good trap. This is actually not the trap we are looking to exploit. Oil trapped at the base of a salt feature is actually very risky and is more often than not a tar ball.

What exploration and appraisal geoscientists are looking for are the traps below the salt. The seismic reflections below the salt are what we map as the traps for oil.

Speaking of seismic reflections, the most prominent one (a boomer, we used to say) below the salt you may see in the data (if it is Gulf of Mexico data) is the top of the Cretaceous Period and used as a consistent marker across the entire Gulf of Mexico. All other reflectors above that are younger than the Cretaceous and where you look for the oil traps.

Top of salt is really easy to pick out and will be an easy reflector to image. However, the base of salt can be very difficult, due to sloped interfaces (dips) and the difficulty of seismic waves to penetrate the salt. Another confounding variable is the (likely) presence of inclusions within the salt.

Salt can be very dirty, it is amorphous and ductile. An analogy is like glacier. It will pick up sediments along the way and trap them inside the salt body. This will further confuse the image below the salt and disrupt the base of salt reflector.
