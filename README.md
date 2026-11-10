# Rosoen RLA Study Hub

A static study page for the three Reasoning Through Language Arts sessions. Students can download each presentation and watch each recording from one page on a phone or computer.

## Contents

- `index.html`: the one-page landing page. Each session is a closed section that opens to show its download buttons. It has no build step.
- `files/`: the PowerPoint presentations. Each file name matches its recording:

| Session | Presentation (in `files/`) | Recording (on Google Drive) |
| --- | --- | --- |
| Tuesday session | `RLA_Tuesday_session_Presentation.pptx` | `RLA_Tuesday_session_Recording.mp4` |
| Session 2 | `RLA_Session_2_Presentation.pptx` | `RLA_Session_2_Recording.mp4` |
| Session 3 | `RLA_Session_3_Presentation.pptx` | `RLA_Session_3_Recording.mp4` |

## Recordings

The recordings are not stored in this repo. The page links to them on Google Drive. Each video must be shared as "Anyone with the link" for the download button to work.

## Publish with GitHub Pages

1. Create an empty repository on GitHub, for example `rosoen-rla-study-hub`.
2. From this folder, connect and push:

   ```
   git remote add origin https://github.com/<your-username>/rosoen-rla-study-hub.git
   git branch -M main
   git push -u origin main
   ```

3. In the repository, open Settings, then Pages. Under Build and deployment, choose "Deploy from a branch", select `main`, and select the `/ (root)` folder.
4. The site will be live at `https://<your-username>.github.io/rosoen-rla-study-hub/` within a few minutes.

## Updating

- To replace a presentation, overwrite the file in `files/` with the same name.
- To change a recording, replace the Google Drive file ID in the matching "Download recording" link in `index.html`. The direct download link has the form `https://drive.google.com/uc?export=download&id=<FILE_ID>`.
- To add a session, copy one `<details class="session">` block in `index.html`, then update its title, description, and the two download links with the next numbers.
